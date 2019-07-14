# Vocal Data

The VocalData is a corpus of lyrics singing voice, separated from songs of professional singers. Its purpose is to enable the training and testing of automatic lyrics recognition (ALR) systems.

More information about the corpus and experiments can be found in [our paper](https://arxiv.org/abs/1804.05306) (In this paper, we only used train_clean and test_clean data).

One can also take a look at the [Demo](https://pascalson.github.io/Transcribing_Lyrics.html).

If you need this corpus for academic use, please email your purpose and institution to:
* Pascal: pascaltuan@gmail.com


## General Information

* A total of 110 songs with 62 different singers
* The total duration is about 313.8 minutes
* Every songs is compressed in `flac` format: (singer-id)-(song-id)-(clip-id).flac
    * train_clean, test_clean : WER < 95% by ASR trained with Librispeech
    * train_other, test_other : WER >= 95% by ASR trained with Librispeech
* Directory `alignment/` contains 13 clips with labeled alignments
* Our experiment for this data is in another repository [Lyric_ASR](https://github.com/jackyyy0228/Lyric_ASR)


## Structures

- SONGS.TXT: singer, clustered genres information of each song.
- SONG_ori.TXT: raw genres information.
- SETS.TXT: the ID list of songs in `train_clean/`, `test_clean/`, `train_other/`, `test_other/`.
- SINGERS.TXT: singer information.
- CLIPS.TXT: duration, labels of singing speed, and harmony existence of each clip.


## Citation

```
@inproceedings{tsai2018transcribing,
  title={Transcribing lyrics from commercial song audio: the first step towards singing content processing},
  author={Tsai, Che-Ping and Tuan, Yi-Lin and Lee, Lin-shan},
  booktitle={2018 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP)},
  pages={5749--5753},
  year={2018},
  organization={IEEE}
}
```


## Other Singing Voice Data Websites
- [DAMP](https://ccrma.stanford.edu/damp/): cover songs corpus
- [Kara1k](http://yannbayle.fr/karamir/kara1k.php): cover songs corpus
- [Singing Voice Audio Dataset](http://isophonics.net/SingingVoiceDataset): Opera songs by professional and amateur singers
- [A list of data related to music information retrieval](https://www.audiocontentanalysis.org/data-sets/)
