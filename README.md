# Liang Shiqiu's Taiwan-Period Writings

This repository documents Liang Shiqiu's (梁实秋／梁實秋) literary and scholarly work in Taiwan from 1949 to 1987. It combines a source chronology, two research-oriented timelines, and a short academic paper that reads his Taiwan period through the relationships among his essays, Shakespeare translations, dictionaries, teaching materials, memoirs, and works of literary history.

The repository is intended for literary research, teaching, and bibliographic reference. Most of its contents are in Chinese.

## Start here

- [梁实秋台湾时期作品年表_简表版.md](梁实秋台湾时期作品年表_简表版.md) is the quickest introduction. It lists major works and events by year across five periods.
- [梁实秋台湾时期作品年表_完整版.md](梁实秋台湾时期作品年表_完整版.md) adds publication details, biographical context, interpretive notes, source citations, and points where the evidence remains uncertain.
- [臺灣現當代作家研究資料彙編收存系統_梁實秋文學年表.md](臺灣現當代作家研究資料彙編收存系統_梁實秋文學年表.md) preserves the underlying National Museum of Taiwan Literature chronology in Traditional Chinese, with corrections to obvious transcription errors and a documented 1979 addition from National Taiwan Normal University.
- [paper/main.pdf](paper/main.pdf) is the compiled paper, *从《雅舍小品》到〈還鄉〉：梁实秋台湾时期作品小传*.

## Research scope

The timelines organize Liang's Taiwan years into five working periods:

| Period | Years | Focus |
| --- | --- | --- |
| Arrival and resettlement | 1949-1952 | Migration to Taiwan, *Sketches of a Cottager* (《雅舍小品》), and early institutional work |
| Translation and teaching | 1953-1966 | Shakespeare translation, dictionaries, textbooks, and National Taiwan Normal University |
| Completion and renewed essay writing | 1967-1973 | The forty-volume Shakespeare project, literary memory, travel writing, and the return of the "Yashe" series |
| Bereavement and readjustment | 1974-1976 | *Memories of Huaiyuan* (《槐園夢憶》), remarriage, and the "Siyixuan" essays |
| Late work | 1977-1987 | Essays, food writing, English literary history, collected works, and the posthumous essay 〈還鄉〉 |

This periodization is an interpretive research framework, not a claim that Liang's work falls into five sharply separated phases. The fuller chronology explicitly labels inference, conflicting dates, and details that still require verification.

## Repository layout

```text
.
├── 梁实秋台湾时期作品年表_简表版.md       # Concise annual index
├── 梁实秋台湾时期作品年表_完整版.md       # Expanded research chronology
├── 臺灣現當代作家研究資料彙編收存系統_梁實秋文學年表.md
│                                             # Corrected source chronology
└── paper/
    ├── main.tex                              # Paper source
    ├── main.pdf                              # Compiled paper
    ├── references.bib                        # BibLaTeX bibliography
    ├── Makefile                              # Local build helper
    └── figures/                              # Figure source and attribution notes
```

## Building the paper

The committed PDF can be read directly. To rebuild it, install:

- XeLaTeX and `latexmk`
- Biber
- the `ctex` and `biblatex-gb7714-2015` LaTeX packages
- Noto Serif CJK SC, Noto Sans CJK SC, and Noto Sans Mono CJK SC

Then run:

```bash
cd paper
latexmk -xelatex -interaction=nonstopmode -file-line-error -outdir=build main.tex
cp build/main.pdf main.pdf
```

The generated paper is an A4 PDF. Bibliographic entries are maintained in [paper/references.bib](paper/references.bib).

## Using and citing the data

The Traditional Chinese chronology is based primarily on the National Museum of Taiwan Literature's [梁實秋文學年表](https://cws.nmtl.gov.tw/home/zh-tw/chronology/585801), supplemented where noted by the National Taiwan Normal University Liang Shiqiu Residence chronology and published scholarship.

For academic use:

1. Treat the source chronology, expanded chronology, and interpretive paper as distinct layers.
2. Follow the inline source notes to the original publication or institutional record whenever possible.
3. Preserve conflicting accounts rather than silently selecting one; the repository currently notes, for example, discrepancies in the date of Liang's 1982 family reunion and in accounts of his cause of death.
4. Mark new interpretive claims as analysis rather than bibliographic fact.

The source chronology uses Traditional Chinese. The derived timelines and paper mainly use Simplified Chinese, while original titles and quotations retain their published forms where appropriate.

## Contributing

Corrections and additions should include a traceable source: author or institution, title, publication, date, and a stable URL or page number when available. Please note whether a change corrects a factual record, reconciles a variant, or adds interpretation.

## License

This repository uses a dual-license model:

- Code, scripts, and software utilities are licensed under the [MIT License](LICENSE-MIT).
- Chronologies, documentation, paper sources, prompts, and other written content are licensed under [CC BY-NC-SA 4.0](LICENSE). See [LICENSE-CC-BY-4.0](LICENSE-CC-BY-4.0) for the full license text included in the repository.

Third-party source material remains subject to its original copyright and terms of use.
