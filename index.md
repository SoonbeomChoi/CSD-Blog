---
title: "CSD: Children's Song Dataset for Singing Voice Research"
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
    table-layout:fixed;
    width: 100%;
    overflow: hidden;
}
#player{
    width: 100%;
}
</style>

## Overview
<p align="justify">
We introduce the Children's Song Dataset (CSD) which contains vocal recordings of 100 children's songs in Korean or English. The audio recordings are precisely aligned with the MIDI transcriptions and lyrics annotations and so we expect that the dataset can be useful for various singing voice analysis and synthesis tasks. 
</p>

## Dataset Contents
<p align="justify">
The dataset is composed of 50 Korean and 50 English songs sung by a Korean female professional pop singer. Each song is recorded in two separate keys, ranging from 3 to 5 semitones, resulting in a total of 200 audio recordings. We collected the children's songs to avoid the possible copyright issues in commercial pop music. 25 songs are recorded in both Korean and English.

Each audio recording is paired with a MIDI transcription file and a lyrics annotation file. We annotated the note onset and duration with consistent guide lines throught various expressions.
</p>

## MIDI and Lyric Annotation

## Samples
CSD dataset is recorded in both English and Korean. Some songs are recorded in both Korean and English and they have same meanings. Those samples are shown as below.

<table>
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

