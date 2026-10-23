<p align="center"><img src="images/icon.png" width="128" alt="Ringout icon"></p>

<h1 align="center">Ringout</h1>
<p align="center"><b>Guitar practice that listens.</b><br>
Scales, timing, backing tracks and songs, with every note you play judged in real time.<br>
<sub>macOS · Windows (preview) · English / 한국어 · free</sub></p>

<p align="center">
  <a href="https://github.com/kita-ikuyo-star/Ringout-Guitar-Practice/releases/latest/download/Ringout-1.1.0.dmg"><b>Download for Mac (.dmg)</b></a> ·
  <a href="https://github.com/kita-ikuyo-star/Ringout-Guitar-Practice/releases/latest/download/Ringout-1.1.0-windows-x64.zip"><b>Download for Windows (.zip, preview)</b></a> ·
  <a href="https://github.com/kita-ikuyo-star/Ringout-Guitar-Practice/releases">All releases</a>
</p>

![Scale practice: the fretboard shows the whole scale, the current position and the note to play now](images/scale.png)

Ringout lights up **the note to play now** on the fretboard, in time with a metronome, drums or a backing track,
and listens to your guitar to tell you whether you hit it: right note, wrong note or missed, and how early or late.

## Features

### Practise scales the way you'd practise with a teacher
- Minor/major pentatonic (5 boxes or 3 notes per string), blues, natural minor/major, the modes (Dorian to Locrian), harmonic and melodic minor, chromatic. All 12 keys; standard, half-step-down and drop D tuning.
- One position, linked positions, one string, or two strings across the whole neck.
- Patterns: up, down, up-and-back, groups of 3 and 4, thirds, random order, and practice phrases written for the app.
- Moves to the next position or a new key every N laps; **suggested practice** for each scale in a sensible learning order.

### Hear-and-judge
- Real-time pitch detection judges every beat: hit / wrong / missed, accuracy, streak and timing error.
- Latency compensation, an "ignore octave" option, and a strobe/needle tuner (A4 = 430–450 Hz).
- **Bend trainer** (¼ to 1½ tones, measured in cents) and **vibrato trainer** (rate in time with the tempo, target width, pitch graph).
- Arpeggios and CAGED shapes, and fretboard quizzes (find the note, name the note, intervals, ear training).

### Timing
- Sample-accurate metronome from 30 to 300 BPM, simple and compound meters (2/4–7/4, 3/8–12/8), subdivisions, count-in, tap tempo.
- Drum grooves (rock, shuffle, half-time, funk, one drop, slow blues, waltz and more).
- Rhythm training: clicks only on 2 & 4 or off-beats, and gap clicks (bars of silence while judging continues).
- Speed training: +BPM every N laps, and fretboard hints that fade away as you improve.

### Backing tracks
![Backing track: chord tones of the current chord on the fretboard](images/backing.png)
- 17 built-in tracks (blues, minor blues, pop, rock, funk, reggae, disco, ballad, waltz…) with chords, bass and drums written for the app. Change key and tempo freely, or build your own.
- **Chord-tone targets**: any chord tone, root, 3rd, 5th, 7th, guide tones, or rotating. Chords and double stops are checked so the app can tell you which note was missing.

### Songs
![Songs: Guitar Pro tab with score and the fretboard](images/songs-tab.png)
- Open **Guitar Pro 7/8 (.gp)** tabs: score and tab view, repeats and codas unrolled, every note judged, playback at 25–150 %, loops that speed up each pass, and built-in guitar playback.
- Learn from **audio files** (MP3, M4A, WAV, AIFF, FLAC): change speed without changing pitch, shift pitch ±12 semitones, seamless A–B loops, markers.
- **Record** your guitar and the backing as separate tracks, listen back and export a mix.

### Track your progress
![Practice log with calendar](images/log.png)
- Every session is logged automatically: time, BPM, accuracy and the spots you miss most.
- A calendar coloured by accuracy, your best tempo for each exercise, and "practise this again" suggestions.
- Ready-made **practice routines** (25, 35 and 43 minutes), or build your own.

### Sound and gear
- Choose input and output devices and the input channel; monitoring; buffer sizes down to 32 frames.
- Built-in guitar sound with amp and cabinet voicing (clean, overdrive, distortion, acoustic).
- Plugin chains for your guitar input and the app's instruments: **Audio Unit** on Mac, **VST3** on Windows. Judging always uses the clean input, and the metronome never goes through the plugins.

## Requirements

| | Mac | Windows (preview) |
|---|---|---|
| System | macOS 14 Sonoma or later, Apple silicon (M1 or later) | Windows 10 or 11, 64-bit |
| Audio | Audio interface with an instrument (Hi-Z) input recommended; headphones recommended | Same. WASAPI (shared or exclusive) |
| Download | `Ringout-1.1.0.dmg` | `Ringout-1.1.0-windows-x64.zip` |

A microphone works too, but a metronome playing through speakers into a microphone confuses the pitch detection, so use headphones.

## Install

**Mac**
1. Open the .dmg and drag **Ringout** into **Applications**.
2. The app isn't signed with an Apple Developer ID, so macOS blocks it the first time. Open it once, click **Done**, then go to **System Settings → Privacy & Security** and click **Open Anyway**.
3. Allow microphone (audio input) access when asked. The app uses it to hear your guitar.

**Windows (preview)**
1. Unzip the folder anywhere and run `Ringout.exe`. Nothing else gets installed.
2. The app isn't code-signed, so SmartScreen may say "Windows protected your PC". Click **More info → Run anyway**.

> The Windows version is a **preview**. It is built from the same code as the Mac app but hasn't been tested on Windows PCs yet. Please report any problems in [Issues](https://github.com/kita-ikuyo-star/Ringout-Guitar-Practice/issues).

**Check your download** (optional): compare with `SHA256SUMS.txt` on the release page.
Mac: `shasum -a 256 Ringout-1.1.0.dmg` · Windows: `certutil -hashfile Ringout-1.1.0-windows-x64.zip SHA256`

## Privacy

- Ringout **never connects to the internet**. There are no accounts, analytics, ads or update checks.
- Your practice history, routines, settings and recordings stay on your computer:
  `~/Library/Application Support/GuitarPractice` (Mac) or `%APPDATA%\GuitarPractice` (Windows).
- Audio input is used only to detect pitch, and is saved to a file only when you press **Record**.

## Licence

- **Ringout is freeware**: free to use for practice and teaching, provided as is with no warranty. You may not sell it or distribute modified copies. Please share this page rather than the files. Full terms: [LICENSE.txt](LICENSE.txt).
- The app includes third-party components under their own licences: the VST3 SDK (MIT, Windows only), the Bravura music font outlines (SIL OFL 1.1) and playback-order rules ported from alphaTab (MPL 2.0). See [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md). The full licence texts, and the MPL-covered source files as that licence requires, are included in each download.
- This repository only distributes the app. The app's own source code isn't published.
- VST and ASIO are trademarks of Steinberg Media Technologies GmbH. Guitar Pro is a trademark of Arobas Music. Ringout isn't affiliated with either company.

## Feedback

Found a bug or have an idea? Open an [issue](https://github.com/kita-ikuyo-star/Ringout-Guitar-Practice/issues). Please don't attach recordings or files that contain personal information.

---

## 한국어

**Ringout(링아웃)** 은 메트로놈·드럼·백킹 트랙에 맞춰 지판에 지금 칠 음을 보여 주고, 기타 소리를 듣고 맞게 쳤는지 바로 판정하는 무료 기타 연습 앱입니다. 화면은 한국어·영어를 지원합니다.

- **스케일**: 펜타토닉(5박스·3NPS)·블루스·메이저/마이너·모드·하모닉/멜로딕 마이너·크로매틱, 포지션 잇기·한 줄·두 줄, 시퀀스·3도·랜덤·프레이즈, 스케일별 추천 연습
- **판정**: 박마다 맞음/틀림/놓침, 정확도·연속 기록·타이밍, 지연 보정, 튜너, 벤딩·비브라토 연습, 아르페지오·CAGED, 지판 퀴즈
- **박자**: 30–300 BPM 메트로놈, 여러 박자표, 드럼 패턴, 리듬 훈련(2·4박, 엇박, 갭 클릭), 속도 훈련
- **백킹 트랙**: 내장 17개와 직접 만들기, 코드톤 판정, 더블스톱·코드 전체 화음 확인
- **곡**: Guitar Pro 7·8(.gp) 타브·악보 따라치기, 오디오 파일 속도·음높이 조절과 구간 반복, 기타·반주 따로 녹음
- **기록**: 자동 연습 기록, 정확도 색 달력, 연습 루틴
- **소리**: 장치·채널 선택, 내장 기타 소리(앰프·캐비닛), 플러그인(Mac AU, Windows VST3)

**내려받기**: 위의 Mac(.dmg) 또는 Windows(.zip, 미리 보기) 링크.
Mac은 처음 열 때 **시스템 설정 → 개인정보 보호 및 보안 → 그래도 열기**, Windows는 SmartScreen에서 **추가 정보 → 실행**을 누르세요.

**개인정보**: 인터넷에 연결하지 않으며, 기록·설정·녹음은 이 컴퓨터에만 저장됩니다.
**이용 조건**: 무료(프리웨어), 판매·고친 판 배포 금지. 자세한 내용은 [LICENSE.txt](LICENSE.txt), 오픈소스 고지는 [THIRD-PARTY-NOTICES.md](THIRD-PARTY-NOTICES.md).

<sub>© 2026 Ringout</sub>
