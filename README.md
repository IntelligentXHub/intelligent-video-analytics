# Chapter 1: Introduction to CCTV and Its Devices

**Intelligent Video Analytics: Surveillance, Safety, and Operational Efficiency**  
Mahendra, Adinandra and Wisudawan. Mercury Learning and Information.  
**Book reference:** Chapter 1, printed pages 1 to 21.  
**Companion site:** www.intelligentxhub.com

## About this chapter

Chapter 1 introduces the evolution of CCTV, its applications and principal components. It explains camera types, lenses, recording devices, recording strategies, storage estimation, retention, metadata and monitoring displays. These topics establish the hardware and operational foundation for the networking and intelligent analytics chapters that follow.

## Chapter 1 files

| File | Description | How to use |
| --- | --- | --- |
| [Lecture_Slides_Ch01.pptx](Lecture_Slides_Ch01.pptx) | Editable textbook-style lecture slides with Chapter 1 page references and book figures | Use during lectures and classroom discussions |
| [CCTV_Storage_Calculator.xlsx](CCTV_Storage_Calculator.xlsx) | Formula-driven capacity calculator with a worked book scenario, configurable assumptions and reference tables | Change blue input cells and examine capacity requirements |
| [CCTV_Storage_Lab.ipynb](CCTV_Storage_Lab.ipynb) | Python notebook on retention, recording duty cycle, camera inventory, capacity and synthetic metadata search | Run all cells in Google Colab or Jupyter |
| [Exercises_Ch01.pdf](Exercises_Ch01.pdf) | Conceptual, computational and engineering exercises | Use individually or as an assignment |

## Suggested learning sequence

1. Read Chapter 1 of the textbook, printed pages 1 to 21.
2. Review the lecture slides and identify major camera, lens and recorder categories.
3. Open the Excel calculator. Change the camera count, bit rate and retention period.
4. Run the notebook and compare recording schedules, storage scenarios and metadata queries.
5. Complete the student exercises. State assumptions and report units accurately.

## Expected learning outcomes

By the end of this chapter, readers should be able to:

- Explain the main components and application areas of CCTV systems.
- Distinguish analog/IP cameras and DVR/NVR/HVR recording devices.
- Select plausible recording modes for different operational settings.
- Estimate basic storage capacity and explain the effect of recording duty cycle and retention.
- Explain why retention policies and metadata indexing matter.

## Numerical note: storage units

The textbook introduces a baseline calculation on page 16 that divides by 8 and 1024. This is reproduced as a **book-style capacity estimate** for teaching continuity. However, a Mbps rate uses decimal megabits per second, and this shorthand is not a dimensionally exact conversion to either decimal GB or binary GiB. The materials therefore report an exact decimal GB calculation and a separate GiB value.

For one 2 Mbps stream recorded continuously for 30 days:

- Book-style expression, `2 * 3600 * 24 * 30 / (8 * 1024)`: **632.8125** (book-style GB).
- Exact decimal storage: `2,000,000 * 86,400 * 30 / 8 / 1,000,000,000`: **648 GB**.
- Exact binary storage: `648,000,000,000 / 1,073,741,824`: **603.50 GiB**.

The book prints approximately 633.79 GB for its worked example. The companion treats this as a numerical discrepancy rather than silently reproducing the result. The values are theoretical recording payloads; equipment sizing also requires allowances for system overhead, reserve capacity, redundancy and vendor-specific behavior.

## Scope and prerequisites

The notebook requires Python 3 and standard packages available in Google Colab. No camera, network recorder, external API, cloud account or GPU is needed. All event metadata is synthetic. The calculator does not estimate file-system overhead, RAID fault tolerance or actual variable bit rate from a specific camera. Results must be validated against equipment data and deployment constraints before procurement.

## Image and copyright notes

The lecture slides contain selected figures from the textbook for review with the publisher's permission to be confirmed before public redistribution. The notebook, workbook and exercises are newly authored companion materials. Do not upload the entire textbook PDF to this repository. The use of a textbook figure in this draft is not a statement that online redistribution rights have been granted.

## License and updates

Companion files are supplied for education and evaluation. A definitive software/content license should be added to the repository after confirming the publisher agreement and author rights. File issues with a reproducible example, the affected file, the expected result and your actual result.

www.intelligentxhub.com
