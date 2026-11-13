# Gunparade-March-Korean-Fan-Translation
고기동환상 건퍼레이드 마치의 한국어 팬 번역 및 개조
<img width="1593" height="896" alt="高機動幻想　ガンパレード・マーチ 2026-11-13-17-07-51" src="https://github.com/user-attachments/assets/82821f26-ef48-4eb0-bf7e-327463b828de" />

건퍼레이드 마치 한국어 패처

무수정 일본판 원본 BIN에 적용하는 오프라인 패처입니다. 원본 게임은 포함하지 않습니다.

1. 이 폴더의 GPM_Korean_Patcher.html을 데스크톱 브라우저에서 엽니다.
2. 원본 BIN을 고른 뒤 적용 버튼을 누릅니다. 파일을 업로드하지 않습니다.
3. 검증 후 내려받은 ZIP을 새 폴더에 풉니다.
4. 먼저 ZIP 안의 와이드스크린 설정.bat을 실행합니다. 포터블 버전은 아래 별도 데이터 폴더 설치 방법을 따릅니다.
5. ZIP 안의 CUE로 실행합니다. BIN과 CUE 이름은 바꾸지 마세요.

지원 원본: 440,372,016B, SHA-256 `981218fe0cc29721fa7943ea4985c4a144e548fa27e35fbae691ecbd48b2a0b4`.
파일명이 달라도 크기/해시가 같으면 지원합니다. ZIP/ISO/CUE/이전 패치 적용본은 지원하지 않습니다.

Python 3.10 이상에서는 패처 폴더에서 다음 명령을 쓸 수 있습니다.

    python apply_patch.py "원본 BIN 경로"

`--verify-only`는 쓰기 없이 재구성만 검증합니다. `--output "새이름.bin"`도 지원하며 해당 이름에 맞는 CUE를 만듭니다. 원본과 기존 BIN/CUE는 덮어쓰지 않습니다.

결과 BIN: 443,615,424B, SHA-256 `0c9af444f63e664aacb95fd3d7c4bdfa533c0e9fac858794e9d6998b2edd3825`.

사용자가 전체 진행을 플레이 검증했습니다. 전원 PC 플레이 등 개조 기능은 확인하지 않았습니다. 세부 상태는 manifest.json과 PATCHER_QA.json을 확인하세요.

## 와이드스크린

DuckStation 전용 16:9 와이드스크린 패치입니다. 폭이 부족한 176개 배경과 4:3 그림은 원래 비율과 좌우 여백을 유지합니다.
게임별 화면 비율 16:9, 24비트 영상 4:3 유지, 내장 와이드스크린 핵 끄기, 콘솔의 8MB RAM 켜기를 적용해 주세요.
필드 성능 보정용으로 이 게임의 가상 CPU 클록 150%를 함께 적용합니다.
대사 글자 떨림을 줄이기 위해 내부 해상도 4배, 최근접 텍스처 필터, 확대 텍스처 좌표 반올림을 함께 적용합니다.
기본 설치형 DuckStation은 ROM을 열기 전에 동봉한 와이드스크린 설정.bat을 실행해 주세요. 기존 게임별 설정은 보존됩니다.
명령으로 설치하려면 python install_widescreen_settings.py 를 실행하세요. Windows 기본 데이터 폴더에 적용됩니다.
포터블 버전 등 별도 데이터 폴더를 사용한다면 다음 명령을 사용하세요.

python install_widescreen_settings.py "DuckStation 데이터 폴더"

설정 파일이 없는 경우 SCPS-10136.ini를 데이터 폴더의 gamesettings에 복사해도 됩니다.
설정 후 게임을 완전히 종료하고 다시 시작해 주세요. 이전 버전의 강제 저장 상태 대신 게임 내 저장 데이터를 사용해 주세요.
사용자가 전체 진행을 플레이 검증했습니다. 전원 PC 플레이 등 개조 기능은 확인하지 않았습니다.

## 이미지 글꼴

날짜·요일·날씨·숫자 그림 28개와 지도 지명 그림 23개는 Noto Sans KR ExtraBold를 사용했습니다.
출처: https://github.com/google/fonts/tree/main/ofl/notosanskr

Copyright 2014-2021 Adobe (http://www.adobe.com/), with Reserved Font Name 'Source'

This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is copied below, and is also available with a FAQ at:
https://scripts.sil.org/OFL


-----------------------------------------------------------
SIL OPEN FONT LICENSE Version 1.1 - 26 February 2007
-----------------------------------------------------------

PREAMBLE
The goals of the Open Font License (OFL) are to stimulate worldwide
development of collaborative font projects, to support the font creation
efforts of academic and linguistic communities, and to provide a free and
open framework in which fonts may be shared and improved in partnership
with others.

The OFL allows the licensed fonts to be used, studied, modified and
redistributed freely as long as they are not sold by themselves. The
fonts, including any derivative works, can be bundled, embedded, 
redistributed and/or sold with any software provided that any reserved
names are not used by derivative works. The fonts and derivatives,
however, cannot be released under any other type of license. The
requirement for fonts to remain under this license does not apply
to any document created using the fonts or their derivatives.

DEFINITIONS
"Font Software" refers to the set of files released by the Copyright
Holder(s) under this license and clearly marked as such. This may
include source files, build scripts and documentation.

"Reserved Font Name" refers to any names specified as such after the
copyright statement(s).

"Original Version" refers to the collection of Font Software components as
distributed by the Copyright Holder(s).

"Modified Version" refers to any derivative made by adding to, deleting,
or substituting -- in part or in whole -- any of the components of the
Original Version, by changing formats or by porting the Font Software to a
new environment.

"Author" refers to any designer, engineer, programmer, technical
writer or other person who contributed to the Font Software.

PERMISSION & CONDITIONS
Permission is hereby granted, free of charge, to any person obtaining
a copy of the Font Software, to use, study, copy, merge, embed, modify,
redistribute, and sell modified and unmodified copies of the Font
Software, subject to the following conditions:

1) Neither the Font Software nor any of its individual components,
in Original or Modified Versions, may be sold by itself.

2) Original or Modified Versions of the Font Software may be bundled,
redistributed and/or sold with any software, provided that each copy
contains the above copyright notice and this license. These can be
included either as stand-alone text files, human-readable headers or
in the appropriate machine-readable metadata fields within text or
binary files as long as those fields can be easily viewed by the user.

3) No Modified Version of the Font Software may use the Reserved Font
Name(s) unless explicit written permission is granted by the corresponding
Copyright Holder. This restriction only applies to the primary font name as
presented to the users.

4) The name(s) of the Copyright Holder(s) or the Author(s) of the Font
Software shall not be used to promote, endorse or advertise any
Modified Version, except to acknowledge the contribution(s) of the
Copyright Holder(s) and the Author(s) or with their explicit written
permission.

5) The Font Software, modified or unmodified, in part or in whole,
must be distributed entirely under this license, and must not be
distributed under any other license. The requirement for fonts to
remain under this license does not apply to any document created
using the Font Software.

TERMINATION
This license becomes null and void if any of the above conditions are
not met.

DISCLAIMER
THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT
OF COPYRIGHT, PATENT, TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL THE
COPYRIGHT HOLDER BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
INCLUDING ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL
DAMAGES, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM
OTHER DEALINGS IN THE FONT SOFTWARE.

그 밖의 작은 UI 그림 글자는 MGalmuri v1.1.0 Regular를 사용했습니다. 글꼴 파일 자체는 이 패처에 포함하지 않습니다.
출처: https://github.com/MonadABXY/mgalmuri-font/releases/tag/v1.1.0

Copyright (c) 2026 Monad ABXY (https://monadabxy.com)
Copyright (c) 2019-2025 Lee Minseo (quiple@quiple.dev)

MGalmuri is a modified version of Galmuri by Lee Minseo (quiple).

This Font Software is licensed under the SIL Open Font License, Version 1.1.
This license is copied below, and is also available with a FAQ at:
https://openfontlicense.org


-----------------------------------------------------------
SIL OPEN FONT LICENSE Version 1.1 - 26 February 2007
-----------------------------------------------------------

PREAMBLE
The goals of the Open Font License (OFL) are to stimulate worldwide
development of collaborative font projects, to support the font creation
efforts of academic and linguistic communities, and to provide a free and
open framework in which fonts may be shared and improved in partnership
with others.

The OFL allows the licensed fonts to be used, studied, modified and
redistributed freely as long as they are not sold by themselves. The
fonts, including any derivative works, can be bundled, embedded,
redistributed and/or sold with any software provided that any reserved
names are not used by derivative works. The fonts and derivatives,
however, cannot be released under any other type of license. The
requirement for fonts to remain under this license does not apply
to any document created using the fonts or their derivatives.

DEFINITIONS
"Font Software" refers to the set of files released by the Copyright
Holder(s) under this license and clearly marked as such. This may
include source files, build scripts and documentation.

"Reserved Font Name" refers to any names specified as such after the
copyright statement(s).

"Original Version" refers to the collection of Font Software components as
distributed by the Copyright Holder(s).

"Modified Version" refers to any derivative made by adding to, deleting,
or substituting -- in part or in whole -- any of the components of the
Original Version, by changing formats or by porting the Font Software to a
new environment.

"Author" refers to any designer, engineer, programmer, technical
writer or other person who contributed to the Font Software.

PERMISSION & CONDITIONS
Permission is hereby granted, free of charge, to any person obtaining
a copy of the Font Software, to use, study, copy, merge, embed, modify,
redistribute, and sell modified and unmodified copies of the Font
Software, subject to the following conditions:

1) Neither the Font Software nor any of its individual components,
in Original or Modified Versions, may be sold by itself.

2) Original or Modified Versions of the Font Software may be bundled,
redistributed and/or sold with any software, provided that each copy
contains the above copyright notice and this license. These can be
included either as stand-alone text files, human-readable headers or
in the appropriate machine-readable metadata fields within text or
binary files as long as those fields can be easily viewed by the user.

3) No Modified Version of the Font Software may use the Reserved Font
Name(s) unless explicit written permission is granted by the corresponding
Copyright Holder. This restriction only applies to the primary font name as
presented to the users.

4) The name(s) of the Copyright Holder(s) or the Author(s) of the Font
Software shall not be used to promote, endorse or advertise any
Modified Version, except to acknowledge the contribution(s) of the
Copyright Holder(s) and the Author(s) or with their explicit written
permission.

5) The Font Software, modified or unmodified, in part or in whole,
must be distributed entirely under this license, and must not be
distributed under any other license. The requirement for fonts to
remain under this license does not apply to any document created
using the Font Software.

TERMINATION
This license becomes null and void if any of the above conditions are
not met.

DISCLAIMER
THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT
OF COPYRIGHT, PATENT, TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL THE
COPYRIGHT HOLDER BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
INCLUDING ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL
DAMAGES, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM
OTHER DEALINGS IN THE FONT SOFTWARE.
