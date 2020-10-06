---
title: "CSD: Children's Song Dataset for Singing Voice Research"
description: Music and Audio Computing Lab, KAIST
---

<script>
function pauseOthers(ele) {
    $("audio").not(ele).each(function (index, audio) {audio.pause();});
}
</script>

<style>
.main-content table {
    display: inline-table;
}
table {
    table-layout: auto;
    width: 100%;
    overflow: hidden;
}
#player{
    width: 100%;
}
</style>

![Singing-05](https://user-images.githubusercontent.com/15067112/95196354-e20f0200-0812-11eb-91c3-f53f8d79a535.png)

## Overview
<p align="justify">
We introduce the Children's Song Dataset (CSD) which contains vocal recordings of 100 children's songs in Korean or English. The audio recordings are precisely aligned with the MIDI transcriptions and lyrics annotations and so we expect that the dataset can be useful for various singing voice analysis and synthesis tasks. 
</p>

## Dataset Contents
<p align="justify">
The dataset is composed of 50 Korean and 50 English songs sung by a Korean female professional pop singer. Each song is recorded in two separate keys, ranging from 3 to 5 semitones, resulting in a total of 200 audio recordings. We collected the children's songs to avoid the possible copyright issues in commercial pop music Each audio recording is paired with a MIDI transcription file and a lyrics annotation file.
</p>

<table>
  <tr>
    <th align="left"> Lanauge (number of songs) </th>
    <td align="left"> Korean (50), English (50) </td>
  </tr>
  <tr>
    <th align="left"> Number of keys per song </th>
    <td align="left"> 2 </td>
  </tr>
  <tr>
    <th align="left"> Pitch range </th>
    <td align="left"> F3 - F5 </td>
  </tr>
  <tr>
    <th align="left"> Audio </th>
    <td align="left"> 44.1Hz, 16bit in Wav format </td>
  </tr>
  <tr>
    <th align="left"> MIDI </th>
    <td align="left"> Monophonic MIDI without any expressions </td>
  </tr>
  <tr>
    <th align="left"> Lyrics </th>
    <td align="left"> Grapheme level annoation in a plain TXT format </td>
  </tr>
</table>
<p align="center">Table.1 The summary of CSD dataset.</p>

## MIDI and Lyric Annotation
<p align="justify">
The MIDI data consists of monophonic notes. Each note contains onset and offset times which were manually fine-tuned along with the corresponding syllable. We annotated the note onset and duration with consistent guide lines throught various expressions without any expression data or control change messages.
</p>
<br/>
<p align="justify">
Lyrics are annotated in grapheme level with a plain text format. Each syllable matches with one note and when a syllable corresponds to multiple notes, it is replicated.
</p>

## Samples
<p align="justify">
CSD dataset is recorded in both English and Korean. Some songs are recorded in both Korean and English and they have same meanings. Those samples are shown as below.
</p>

<table style="table-layout: fixed;">
    <tr>
        <th> Song </th>
        <th> English </th>
        <th> Korean </th>
    </tr>
    <tr>
        <th> Twinkle Twinkle <br> Little Star <br> 작은 별 </th> 
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/little_star_en.mp3" type="audio/mpeg"></audio></th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/little_star_kr.mp3" type="audio/mpeg"></audio></th>
    </tr>
    <tr>
        <th> Bingo <br> 빙고 </th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/bingo_en.mp3" type="audio/mpeg"></audio></th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/bingo_kr.mp3" type="audio/mpeg"></audio></th>
    </tr>
    <tr>
        <th> Rudolph the Red <br> Nosed Reindeer <br> 루돌프 </th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/rudolph_en.mp3" type="audio/mpeg"></audio></th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/rudolph_kr.mp3" type="audio/mpeg"></audio></th>
    </tr>
    <tr>
        <th> O Holy Night <br> 오 거룩한 밤 </th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/holynight_en.mp3" type="audio/mpeg"></audio></th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/holynight_kr.mp3" type="audio/mpeg"></audio></th>
    </tr>
    <tr>
        <th> White Christmas <br> 화이트 크리스마스 </th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/white_xmas_en.mp3" type="audio/mpeg"></audio></th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/white_xmas_kr.mp3" type="audio/mpeg"></audio></th>
    </tr>
    <tr>
        <th> Butterfly <br> 나비야 </th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/butterfly_en.mp3" type="audio/mpeg"></audio></th>
        <th> <audio controls id="player" onplay="pauseOthers(this);"><source src="assets/audio/butterfly_kr.mp3" type="audio/mpeg"></audio></th>
    </tr>
</table>

