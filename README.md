# Forensic Voice Comparator

This is a voice comparator which can be used for forensic voice analysis purposes.
This comparator takes in a speaker-unknown voice sample and a known voice sample and outputs the LR (Likelihood Ratio) of the two samples so the result can directly be used in forensic purposes.


# What is Forensic Voice Comparison?

Forensic voice comparison (also referred to as forensic speaker comparison, forensic speaker recognition, and forensic speaker identification), or **FVC**, is the comparison of one or more voice recordings of an unknown speaker to one or more recordings of a known speaker made by a forensic practitioner in order to help the court to identify the criminal.

**A person’s voice is unique** and contains a lot of information, such as where the person grew up and learned to speak, their race and nationality, biological gender, height, and other unique identifiers due to the genuine shape, size, and usage of the person’s vocal organs.


# Forensic Voice Comparison Techniques

There are four basic approaches to forensic voice comparison.
- Auditory
- Spectrographic
- Acoustic-phonetic
- Automatic

The first three approaches can be merged into the Auditory-Acoustic Framework (AAF). 
>These **involve a human practitioner** in the process.

The automatic approach is also called Automatic Speaker Recognition (ASR), Automatic Speaker Comparison, and Automatic Speaker Identification. 
>This approach is **fully automatic**.


## Auditory Approach

In an auditory approach, a forensic practitioner trained in auditory phonetics **listens** to the questioned- and known-speaker recordings. They note the similarities in the sounds they would expect if the sounds were produced by the same speaker and the differences they would expect if they were not.

## Spectrographic Approach

This approach involves making a spectrogram of a word or a phrase from the questioned speaker recording and also making a spectrogram of the same word or a phrase from the suspect speakers (and sometimes foil speakers) recordings.


![This spectrograms show the differences between an American and British female speaker saying the word “master plan”](https://www.phonexia.com/wp-content/uploads/spectrogram-example-forensic-voice-comparison-guide.jpg)

The above spectrograms show the differences between an American and British female speaker saying the word “master plan” (audio taken from Oxford Learner’s Dictionaries). Notice the brightness differences in the sound “a” marked by the white rectangles. The brighter the image, the more sound energy there is at a given time and frequency.


## Acoustic-Phonetic Approach

The acoustic-phonetic approach compares the quantitative measurements of phonetic units’ characteristics in both recordings.

Usually, a practitioner identifies the comparable phonetic units (phonemes, allophones, or the sequences of allophones) of the questioned- and known-speaker’s recordings and measures and compares their parameters..

## Automatic Approach

>**This is the approach we will be using.**

Automatic voice comparison systems – known also as Speaker Identification (SID) or Automatic Speaker Recognition (ASR) – were introduced into forensics in the 2000s when computer systems for voice recognition evolved considerably.

Due to fast signal processing and statistical modeling in ASR systems, thousands of test pairs can be compared very quickly.

In automatic voice comparison systems, spectral measurements are usually made for every short segment, generally from 10 to 30 ms long.

The result of this automatic approach is the **LR**    *(Likelihood Ratio)*.


## Likelihood Ratio (the Result of Automatic Forensic Voice Comparison)

The voice models (voiceprints) of the questioned and known speakers are compared to each other and to a population set model in order to evaluate the ratio between the likelihoods of two hypotheses:

 - The two compared voice recordings were produced by the same speaker
 - The two compared voice recordings were produced by different speakers

>The LR reflects **how much a particular piece of evidence is more likely** under one hypothesis than another.

For mathematical convenience, the result is often presented in the form of Log Likelihood Ratio (LLR) or logarithm (usually decimal or natural) of the likelihood ratio, because the logarithm function is symmetrical about zero:
![](https://www.phonexia.com/wp-content/uploads/score.png)

Thus, high **positive log likelihoods mean the evidence is much more likely to occur under the same-speaker** hypothesis than under the different-speaker hypothesis.

Vice versa, **high negative log likelihoods mean that the evidence is much more likely to occur under the different-speaker** hypothesis than under the same-speaker one. A log likelihood ratio of 0 (or likelihood ratio of 1) means that the evidence cannot support any of the hypotheses.

This results representation fits perfectly with the widely accepted **Bayesian paradigm** of expressing the strength of evidence instead of a binary decision.

