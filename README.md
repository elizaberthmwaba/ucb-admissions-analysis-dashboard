# UC Berkeley Admission Bias Analysis

A Power BI dashboard investigating gender-based admission patterns across six majors at UC Berkeley, using the 1973 graduate admissions dataset. The central question: did UC Berkeley discriminate against female applicants?

The short answer is no, but the data makes a compelling case that it did, until you look closer.

---

## Why This Dataset Matters

In 1973, UC Berkeley was sued for gender bias in graduate admissions. On the surface, the numbers were damning, male applicants were admitted at a rate of **44%** while female applicants were admitted at just **30%**. That is a 14 percentage point gap across 4,839 applications. If you stopped there, you would conclude the university systematically favored men.

But a deeper analysis published in *Science* in 1975 by Bickel, Hammel and O'Connell showed something unexpected. When researchers broke the data down by individual major, the gender gap not only shrank,in several majors, women were actually admitted at *higher* rates than men. The aggregate statistic was not lying, but it was telling the wrong story. This is one of the most cited real-world examples of **Simpson's Paradox** a trend that appears in aggregate data reverses or disappears when the data is broken into subgroups.

This dashboard makes that phenomenon visible and interactive.

---

## The Numbers and What They Actually Mean

### 4,839 applications but the pool is not evenly distributed

Of the 4,839 total applicants, **3,005 (62%) were male and 1,834 (38%) were female**. This imbalance is not incidental, it is the key to understanding everything that follows. The composition of who applies to which major directly shapes the aggregate admission rate, and ignoring it leads to the wrong conclusion.

### 2,068 accepted, but accepted from where?

Of those admitted, the split by major tells the real story. Acceptances were not evenly distributed across majors. Major A alone accounted for a disproportionate share of total applications, and it was also the most competitive Major with the lowest admission rate. Who applied to Major A and in what numbers matters enormously.

### 43% overall admission rate, a misleading headline

A 43% overall admission rate sounds reasonable until you split it by gender. Males were admitted at 44%, females at 30%. That gap looks like bias. But this number is an average across very different majors, and averages across groups with different compositions are dangerous. A hospital that treats more critical patients will always show worse survival rates than one treating minor cases, that does not mean it is a worse hospital. The same logic applies here.


## What the Visuals Reveal

### The donut chart sets up the paradox

62% of applicants were male. But this is not evenly spread across majors. Females concentrated a much higher proportion of their applications in major A the hardest major to get into. Males spread their applications more evenly, including to Majors C, D, E and F, which had significantly higher admission rates. When you average across everyone, males look more successful, not because they were favored, but because they applied to easier majors in greater numbers.

### The applications by major chart shows where the imbalance lives

The applications by major chart  shows that Major A had 108 female applicants versus 1,138 male applicants,a 10:1 ratio. But look at the admission rates for that Major, they are similarly low for both genders. Females were not being rejected from Major A at higher rates than males. They were simply applying to the hardest program in the largest numbers relative to their pool, which dragged their overall rate down. Meanwhile, Major C had 593 female applicants versus 325 male and higher admission rates, contributing more positively to male aggregate rates.

### Where the paradox breaks open

This is the most important visual in the dashboard the admission rate by major chart. When you look at admission rates *within* each major separately, the picture changes completely. In majors C, D and E, female admission rates are comparable to or higher than male rates. In major A, both genders face the same tough odds. There is no major where females are being systematically rejected at a meaningfully higher rate than equivalent male applicants. The discrimination suggested by the headline number does not survive scrutiny at the major level.

### Where offers actually went

The 100% stacked bar makes clear that within each department, the gender split of admitted students roughly tracks the gender split of applicants. No single major shows a dramatic skew toward admitting one gender over the other. If there were systemic bias operating at the departmental level, where actual admissions decisions are made you would expect to see this chart look very different.

---

## The Actual Insight: Structural Inequality, Not Selection Bias

The data does not show that Berkeley's admissions committees were biased against women. It shows something more structural and arguably more important: **women in 1973 were applying to the most competitive, most male-dominated departments in higher numbers**, and those departments admitted very few people regardless of gender.

This raises harder questions than simple selection bias does. Why were women concentrated in the most competitive departments? Were those the ones with the fewest spaces, or the ones with the most cultural barriers already in place? Were women being steered away from the less competitive departments by social or academic norms before they even submitted an application?

The admissions data cannot answer those questions. But it does show that the bias, if any existed, operated upstream of the application not inside the selection process itself. That distinction matters enormously for how an institution responds.

---

## How to Use the Dashboard

- Use the **Gender filter** to isolate the female or male applicant experience across all visuals at once
- Use the **Major filter** to drill into a single department and examine its admission pattern in isolation
- Start with the KPI cards to understand the aggregate picture, then use the major-level charts to interrogate it, the gap between those two views is the entire story

---

## Data Source

- **Dataset**: UC Berkeley graduate admissions, 1973
- **Original source**: Bickel, Hammel & O'Connell (1975) — *Science*, Vol. 187
---

## How to Open

1. Download **Power BI Desktop** for free at [powerbi.microsoft.com](https://powerbi.microsoft.com/desktop)
2. Clone or download this repository
3. Open `admissions-dashboard.pbix` in Power BI Desktop
4. All data is embedded — no external connection required

---

## Author

Built in Power BI Desktop. Analysis and data visualization by **Elizaberth Mwaba**.
