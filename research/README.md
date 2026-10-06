# Aggregate study results

This directory contains summary metrics from an exploratory evaluation of GPT-6 Luna, GPT-6.1 Sol, and GPT-6 Astra on selected closed-ended items from CEP 91 and GSS 2024. It is an aggregate results release, not a complete replication package: row-level profiles, human answers, prompts, and generated responses are not included.

`aggregate-results.csv` has one row per reported model/prompt/context cell. The CEP comparison uses a paired subset of 96 profiles, four items, and five generations per cell (1,920 outputs per cell). The GSS extension uses 24 development profiles, four development-selected items, and three generations (288 outputs per cell). Supervised multinomial rows predict known survey items from a separate training sample; they are not zero-shot LLM results.

`mean_weighted_tv` is the equal-item mean of survey-weighted total variation from the human reference. `mean_weighted_agreement` is the equal-item mean weighted individual agreement where reported. `nonresponse_share` is the mean share of recorded nonresponse categories; for CEP it combines codes -8 and -9, and for the GSS extension it combines DK, REFUSED, and NA. Empty metrics are not reported in the source table. Counts describe generated or predicted outputs, not independent human observations.

The source public-use datasets are available from [Centro de Estudios Públicos](https://www.cepchile.cl/encuesta/encuesta-cep-n-91/) and [NORC's General Social Survey](https://gss.norc.org/get-the-data/stata.html). Their terms govern access and any further use. This file does not redistribute those records. The released summaries match the aggregate values reported in the associated manuscript; because the manuscript is under anonymous review, its bibliographic identity and manuscript file are not included here.

The root MIT License applies to the software. It does not grant rights to the source survey records. No separate license is asserted for these aggregate study summaries; use them with attribution and subject to the source datasets' terms. They should not be interpreted as population-representative estimates or confirmatory model comparisons.
