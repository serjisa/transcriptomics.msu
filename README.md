# Курс «Анализ транскриптомных данных»
На этой странице будут находиться материалы для курса «Анализ транскриптомных данных», который читается в осеннем семестре 2022/2023 учебного года в Московском государственном университете на базе Факультета биоинженерии и биоинформатики. Курс разработан и читается при поддержке [фонда «Интеллект»](https://intellect-foundation.ru/).

## Запись на курс
Курс доступен всем желающим. Более того, в конце курса каждый желающий может получить сертификат (или зачёт, если это студент ФББ МГУ), если выполнит для этого условия (см. ниже). Для того, чтобы записаться на курс, необходимо заполнить [Google-форму](https://forms.gle/rukKz61hRgdvYzzE7) и вступить в [Telegram-чат](https://t.me/transcriptomics_msu).

Занятия проходят по **пятницам с 15:35 до 18:55** по московскому времени (GMT +3). Подключиться к занятиям можно [при помощи Zoom](https://us06web.zoom.us/j/82512958561?pwd=aHZLOHFRNFdiWW43TG9KQ3d6cUdwUT09). Также доступны онлайн YouTube-трансляции (следите за обновлениями на странице [Teach-in](https://www.youtube.com/c/NAUKA0)).

## Программа курса
1. **Лекция**: Технологии секвенирования следующего поколения (NGS). Экспериментальные подходы к секвенированию РНК тканей (bulk RNA-Seq). Сходства и различия с микрочиповыми технологиями. Основные базы данных (SRA, GEO). [Презентация](https://github.com/serjisa/transcriptomics.msu/blob/main/%D0%9B%D0%B5%D0%BA%D1%86%D0%B8%D0%B8/01.%20NGS%20%D0%B8%20RNA-Seq.pdf)<br>
**Семинар**: Базовая работа с прочтениями. SRA-Toolkit, SRA-Explorer, FastQC, MultiQC. [Jupyter-notebook](https://github.com/serjisa/transcriptomics.msu/blob/main/%D0%A1%D0%B5%D0%BC%D0%B8%D0%BD%D0%B0%D1%80%D1%8B/01_%D0%91%D0%B0%D0%B7%D0%BE%D0%B2%D0%B0%D1%8F_%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%B0_%D1%81_%D0%BF%D1%80%D0%BE%D1%87%D1%82%D0%B5%D0%BD%D0%B8%D1%8F%D0%BC%D0%B8.ipynb)<br>
**Запись**: https://www.youtube.com/watch?v=KxkTMlaPp9s

2. **Лекция**: Выравнивания (STAR, HISAT2) и псевдовыравнивания (kallisto, Salmon). EM-алгоритм для оценки представленности транскриптов (RSEM). [Презентация](https://github.com/serjisa/transcriptomics.msu/blob/main/Лекции/02.%20Выравнивания.pdf)<br>
**Семинар**: «препарирование» EM-алгоритма и его реализация на Python. [Jupyter-notebook](https://github.com/serjisa/transcriptomics.msu/blob/main/Семинары/02_EM_алгоритм.ipynb)<br>
**Запись**: https://www.youtube.com/watch?v=LKukq5G8w-M

3. **Лекция**: Основные распределения, встречающиеся в омиксных данных. Методы нормализации в bulk RNA-Seq: от RPKM и TPM до RLE и TMM. Контроль за дисперсией в данных<br>
**Семинар**: Статистические подходы к определению максимально правдоподобных распределений данных

4. **Лекция**: Дифференциальная экспрессия, параметрические и непараметрические тесты. Линейные модели и обобщённые линейные модели (GLM). Работа с экспрессиями на уровне транскриптов. tximport и Sleuth<br>
**Семинар**: Написание собственного алгоритма определения дифференциально экспрессированных генов. Работа с пакетами DESeq2 и edgeR

5. **Лекция**: Системный анализ bulk RNA-Seq: анализ обогащённости (GO Enrichment Analysis), Gene Set Enrichment Analysis (GSEA и ssGSEA). Работа с экспрессионными данными на уровне генных сигнатур. Понятие деконволюции bulk RNA-Seq<br>
**Семинар**: Практическая работа с экспрессионными данными на уровне генных сигнатур. Сравнение различных подходов к определению клеточного состава bulk RNA-Seq (signature-based vs. deconvolution)

6. **Лекция**: Понятие и необходимость scRNA-Seq. Методы подготовки библиотек scRNA-Seq. Сравнение различных подходов для подготовок библиотек для scRNA-Seq. Batch effect в данных scRNA-Seq<br>
**Семинар**: Работа с базами данных scRNA-Seq. Дискуссия на тему правильного выбора стратегии подготовки библиотек. Основы работы с библиотеками scanpy и Seurat

7. **Лекция**: Выравнивания и псевдовыравнивания в scRNA-Seq. Контроль качества клеток в scRNA-Seq. Определение и устранение пустых клеток и дублетов. Очистка от примешавшейя РНК (DecontX)<br>
**Семинар**: Собственная реализация алгоритма поиска пустых капель

8. **Лекция**: Процессинг данных scRNA-Seq: сходства и различия с bulk RNA-Seq. SCTransform, LogNorm, pagoda2 и прочие способы контроля за дисперсией данных<br>
**Семинар**: Собственная реализация алгоритма SCTransform

9. **Лекция**: Проклятие размерности. Feature selection при помощи регуляризаций. Методы feature selection, принятые в scRNA-Seq: выделение высоко-вариабельных генов и подходы к этому выделению. Методы снижения размерности: PCA, t-SNE, UMAP, ForceAtlas2. Графовое представление данных<br>
**Семинар**: Работа с различными методами снижения размерности в scanpy<br>

10. **Лекция**: Подходы к устранению батч-эффекта в scRNA-Seq: Harmony, bbkNN, Scanorama, MNN, conos. Анализ методом канонических корреляций (CCA)<br>
**Семинар**: Сравнение подходов для устранения батч-эффектов в данных scRNA-Seq

11. **Лекция**: Использование вариационных аутоэнкодеров для процессинга scRNA-Seq. scVI-tools<br>
**Семинар**: Препарирование scVI, написание собственного вариационного аутоэнкодера на PyTorch и Pyro

12. **Лекция**: Подходы к кластеризации данных. Иерархическая кластеризация, K-Means, графовые алгоритмы кластеризации (Louvain, Leiden, SNN). Понятие стабильности кластера, бутстрэп<br>
**Семинар**: Реализация алгоритма оценки стабильности кластеров

13. **Лекция**: Определение траекторий дифференцировки клеток в scRNA-Seq: Monocle2, Monocle3, иные подходы. Обобщённые аддитивные модели (GAM) и их использование для определения генов, которые меняют свою экспрессию по ходу дифференцировки клеток. RNA velocity<br>
**Семинар**: Написание собственного алгоритма определения генов, которые меняют свою экспрессию по ходу псевдо-времени</br>

14. **Лекция**: Определение типов клеток в scRNA-Seq: автоматическое и мануальное. Поиск взаимодействий между различными типами клеток, CellPhoneDB<br>
**Семинар**: Написание алгоритма автоматического определения типов клеток. Сравнение существующих алгоритмов

15. **Лекция**: Мультимодальные омики одиночных клеток. Подходы для анализа мультимодальных омик одиночных клеток: MOFA, WNN, totalVI, multiVI. CLR-transformation в омиксных данных. Работа с омиксными данными как с композиционными данными<br>
**Семинар**: Воркшоп по анализу мультимодальных омиксных данных

## Условия зачёта
Критерием успешного освоения курса (зачёт для студентов МГУ или сертификат для свободных слушателей) является выполнение одного из двух условий:
1. выполнение двенадцати и более домашних заданий как минимум на «удовлетворительно»,
2. выполнение двух проектных заданий, которые даются в середине и конце курса.

Формат отчёта по курсу &mdash; ссылка на GitHub-репозиторий с выполненными заданиями (форма для обратной связи будет выложена позднее). Проверяться будут только те работы, которые хотя бы формально могут претендовать на зачёт (т.е. репозитории с 11 и менее домашними заданиями или всего одним проектом **проверяться не будут в принципе**).
