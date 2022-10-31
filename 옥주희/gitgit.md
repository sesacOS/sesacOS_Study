main
➜ sesacOS_Study git:(joohee) git pull
이미 업데이트 상태입니다.
➜ sesacOS_Study git:(joohee) git branch

- joohee
  main
  ➜ sesacOS_Study git:(joohee) git branch -v
- joohee 3b1547f new branch
  main e019a4d [6개 뒤] add 1 person
  ➜ sesacOS_Study git:(joohee) git branch --merged
- joohee
  main
  ➜ sesacOS_Study git:(joohee) git pull
  remote: Enumerating objects: 4, done.
  remote: Counting objects: 100% (4/4), done.
  remote: Compressing objects: 100% (2/2), done.
  remote: Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
  오브젝트 묶음 푸는 중: 100% (2/2), 702 bytes | 234.00 KiB/s, 완료.
  https://github.com/sesacOS/sesacOS_Study URL에서
  4342ac5..ba73497 main -> origin/main
  이미 업데이트 상태입니다.
  ➜ sesacOS_Study git:(joohee) ✗ ls  
  README.md 문승현 옥주희 이태희 정민희 김율리아
  김원석 박보미 이성현 임유빈 정재은
  ➜ sesacOS_Study git:(joohee) ✗ cd 문승현
  ➜ 문승현 git:(joohee) ✗ cat README.md
  ➜ 문승현 git:(joohee) ✗ git pull
  이미 업데이트 상태입니다.
  ➜ 문승현 git:(joohee) ✗ cat README.md
  ➜ 문승현 git:(joohee) ✗ cd ../
  ➜ sesacOS_Study git:(joohee) ✗ cd 이태희/
  ➜ 이태희 git:(joohee) ✗ cat README.md
  ➜ 이태희 git:(joohee) ✗ git pull
  이미 업데이트 상태입니다.
  ➜ 이태희 git:(joohee) ✗ git status
  현재 브랜치 joohee
  브랜치가 'origin/joohee'에 맞게 업데이트된 상태입니다.

커밋하도록 정하지 않은 변경 사항:
(무엇을 커밋할지 바꾸려면 "git add <파일>..."을 사용하십시오)
(use "git restore <file>..." to discard changes in working directory)
수정함: "../\354\230\245\354\243\274\355\235\254/README.md"

커밋할 변경 사항을 추가하지 않았습니다 ("git add" 및/또는 "git commit -a"를
사용하십시오)
➜ 이태희 git:(joohee) ✗ git add .  
➜ 이태희 git:(joohee) ✗ git commit -m "new"
현재 브랜치 joohee
브랜치가 'origin/joohee'에 맞게 업데이트된 상태입니다.

커밋하도록 정하지 않은 변경 사항:
(무엇을 커밋할지 바꾸려면 "git add <파일>..."을 사용하십시오)
(use "git restore <file>..." to discard changes in working directory)
수정함: "../\354\230\245\354\243\274\355\235\254/README.md"

커밋할 변경 사항을 추가하지 않았습니다 ("git add" 및/또는 "git commit -a"를
사용하십시오)
➜ 이태희 git:(joohee) ✗ git status
현재 브랜치 joohee
브랜치가 'origin/joohee'에 맞게 업데이트된 상태입니다.

커밋하도록 정하지 않은 변경 사항:
(무엇을 커밋할지 바꾸려면 "git add <파일>..."을 사용하십시오)
(use "git restore <file>..." to discard changes in working directory)
수정함: "../\354\230\245\354\243\274\355\235\254/README.md"

커밋할 변경 사항을 추가하지 않았습니다 ("git add" 및/또는 "git commit -a"를
사용하십시오)
➜ 이태희 git:(joohee) ✗ cd ..
➜ sesacOS_Study git:(joohee) ✗ ks
zsh: command not found: ks
➜ sesacOS_Study git:(joohee) ✗ ls
README.md 문승현 옥주희 이태희 정민희 김율리아
김원석 박보미 이성현 임유빈 정재은
➜ sesacOS_Study git:(joohee) ✗ cd ..
➜ ssac git:(main) ✗ ls
221025 README.md handout study
ETC class sesacOS_Study 제출서류
➜ ssac git:(main) ✗ rm -rf sesacOS_Study
➜ ssac git:(main) ✗ ls
221025 README.md handout 제출서류
ETC class study
➜ ssac git:(main) ✗ git clone https://github.com/sesacOS/sesacOS_Study.git
'sesacOS_Study'에 복제합니다...
remote: Enumerating objects: 98, done.
remote: Counting objects: 100% (98/98), done.
remote: Compressing objects: 100% (64/64), done.
remote: Total 98 (delta 29), reused 65 (delta 12), pack-reused 0
오브젝트를 받는 중: 100% (98/98), 17.46 KiB | 3.49 MiB/s, 완료.
델타를 알아내는 중: 100% (29/29), 완료.
➜ ssac git:(main) ✗ cd sesacOS_Study
➜ sesacOS_Study git:(main) ls
README.md 문승현 옥주희 이태희 정민희 김율리아
김원석 박보미 이성현 임유빈 정재은
➜ sesacOS_Study git:(main) cd 문승현
➜ 문승현 git:(main) cat README.md
Hello
➜ 문승현 git:(main) git branch

- main
  ➜ 문승현 git:(main) git hist
  git: 'hist'은(는) 깃 명령이 아닙니다. 'git --help'를 참고하십시오.

가장 비슷한 명령은
bisect
➜ 문승현 git:(main) git log
commit ba734978457fdbc081e573ec877ec5b86c90533d (HEAD -> main, origin/main, origin/HEAD)
Merge: 4342ac5 fc5c7db
Author: anstmdgus <47172522+anstmdgus@users.noreply.github.com>
Date: Tue Oct 25 18:50:20 2022 +0900

    Merge pull request #12 from sesacOS/seunghyun

    승현 update

commit fc5c7dbdc9d6873dd0a074a9aef9b46fd22a26a9 (origin/seunghyun)
Author: moon <anstmdgus473@naver.com>
Date: Tue Oct 25 18:49:28 2022 +0900

    승현 update

commit 4342ac5bd56ace7e8018881425fb3ca25e444227 (origin/yubeen)
Merge: a925e1d c7d85da
Author: Been0701 <108451986+Been0701@users.noreply.github.com>
Date: Tue Oct 25 18:48:37 2022 +0900

    Merge pull request #11 from sesacOS/yubeen

    수정 후 커밋

commit a925e1d6b966efe913fd15ae8f1e9e3501513311
Merge: 5307536 068a3b6
Author: taehee <113709273+taeheehi@users.noreply.github.com>
Date: Tue Oct 25 18:46:44 2022 +0900

    Merge pull request #9 from sesacOS/taehee

    hello.html upload

commit 530753648b460d9c21c15608b5168bb265eb99b7
Merge: 1f50a6d 3b1547f
Author: jooheeok <65056196+jooheeOk@users.noreply.github.com>
Date: Tue Oct 25 18:46:27 2022 +0900

    Merge pull request #10 from sesacOS/joohee

    new branch

commit 1f50a6d5b4325e4c340e5f75540be97ae37657a5
Merge: 8690aa9 9ad98fb
Author: sognociel <110799821+sognociel@users.noreply.github.com>
Date: Tue Oct 25 18:45:46 2022 +0900

    Merge pull request #8 from sesacOS/bomi

    test

commit c7d85da08fc27c6f7dab57c78859daf2cbc5b400
Author: Been0701 <dlwptlwkr93@naver.com>
Date: Tue Oct 25 18:45:39 2022 +0900

    수정 후 커밋

commit 068a3b6f6fc31ac3833905c0360af448eda03c50 (origin/taehee)
Author: DESKTOP-O4MJ0GF\LGE <taehi.dev@gmail.com>
Date: Tue Oct 25 18:43:22 2022 +0900

    hello.html upload

commit 8690aa961854f84381dd71844a2cb79452ce5a36
Merge: 3267f04 f0b427d
Author: jeongminhui <62429295+jeongminhui@users.noreply.github.com>
Date: Tue Oct 25 18:41:32 2022 +0900

    Merge pull request #7 from sesacOS/minhee

    upload tes

commit 9ad98fb88901438f195131c7dc6479e34517b952 (origin/bomi)
Author: sognociel <sognociel@gmail.com>
Date: Tue Oct 25 18:40:23 2022 +0900

    test

commit 3267f04d9dfae101f9a26d954eb55c34cee5a246
Merge: 636925d 6390c77
Author: Been0701 <108451986+Been0701@users.noreply.github.com>
Date: Tue Oct 25 18:39:42 2022 +0900

    Merge pull request #6 from sesacOS/yubeen

    first commit

commit 636925d7e7a3662be491aa42b84f12e636f2cd5d
Merge: e019a4d 4666e3f
Author: may-jan <116541435+may-jan@users.noreply.github.com>
Date: Tue Oct 25 18:39:15 2022 +0900

    Merge pull request #5 from sesacOS/jaeeun

    first commit

commit f0b427d383410a3be15b1491b8ad57af4b547fca (origin/minhee)
Author: DESKTOP-881NP36\minhee <jeongminhui0503@gmail.com>
Date: Tue Oct 25 18:38:54 2022 +0900

    upload tes

commit 6390c774f1bc6b9dedcd42f1e0bcddfdc37b18df
Author: Been0701 <dlwptlwkr93@naver.com>
Date: Tue Oct 25 18:38:30 2022 +0900

    first commit

commit 4666e3f97932d7e1bceb9067cde4dc4fbaae104f (origin/jaeeun)
Author: jaeeun <jaeeun9862@gmail.com>
Date: Tue Oct 25 18:38:03 2022 +0900

    first commit

commit 3b1547fca345670b2f371f1b38ac29d9c8e171a8 (origin/joohee)
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 18:37:12 2022 +0900

    new branch

commit e019a4ddbeed61a3e03c3b45bb2e1fcc405bd269
Author: Harimad <leesh68481@gmail.com>
Date: Tue Oct 25 18:21:25 2022 +0900

    add 1 person

commit 66b1920aef723a01bf129bb59870fb9e42667f57
Merge: bc28c11 059af82
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Tue Oct 25 17:42:19 2022 +0900

    Merge pull request #4 from sesacOS/yuuulya

    [YUL] week-1 note upload

commit 059af827eea0ff4807a1c65a0406decef1848fcd (origin/yuuulya)
Author: yuuulya <yla101@naver.com>
Date: Tue Oct 25 17:41:15 2022 +0900

    [YUL] week-1 note upload

commit bc28c117bae3645c1457fc5031218d1b3cd08b89
Merge: 8abfe7e 4bbe657
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:41:18 2022 +0900

    Merge pull request #3 from sesacOS/seongHyeon

    test5

commit 4bbe657819fb13d53037e530c5cfd058d933c6cf (origin/seongHyeon)
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:37:31 2022 +0900

    test5

commit 8abfe7eb1dd23c84137b66be8be83b89b3b3debe
Merge: ec149b6 98d320d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:08:48 2022 +0900

    Merge pull request #2 from sesacOS/seongHyeon

    SH test4

commit 98d320dddbdb3abb58207414f0a883a3bffc68f2
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:06:37 2022 +0900

    SH test4

commit ec149b628354982af299209a7743065c8219f675
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 19:44:03 2022 +0900

    test3

commit 16fca52e013b89b566734e4b5d9b425e518adb61
Merge: e6c4e39 061641c
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Mon Oct 24 19:41:58 2022 +0900

    Merge pull request #1 from sesacOS/yuuulya

    github upload test

commit 061641c4d4533b5c9dacd9a2fbf546084883d0ca
Author: yuuulya <yla101@naver.com>
Date: Mon Oct 24 19:22:51 2022 +0900

    github upload test

commit e6c4e3959ed05213b56594f50ec2b7bc73b7897b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:46:27 2022 +0900

    join 1 people

commit fc0d21785f94ae123cf8fc17eb25b91ee6947bea
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:43:59 2022 +0900

    test2

commit 4bcfa3ad2a627d98625a7826a155d592b5764da3
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:37:22 2022 +0900

    joined 2 people

commit 9aff9ae68bb692fa240f3d199bba0b658ca33846
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:23:11 2022 +0900

    [SH] test

commit 690ca5d29a8ed0308d7158da24dfe8e9ccad59ca
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:21:23 2022 +0900

    Update README.md

commit f096b5c83ac48284ce99383647520a13dd59531d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:00:14 2022 +0900

    Update README.md

commit ba666507be258339b4e5945edbab74bd46a3342b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:12:04 2022 +0900

    made folders & files

commit a085e582a959c0e05e0e815c2ffaa8e8af1c4410
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:03:29 2022 +0900

    Initial commit

➜ 문승현 git:(main) git switch joohee
branch 'joohee' set up to track 'origin/joohee'.
새로 만든 'joohee' 브랜치로 전환합니다
➜ 문승현 git:(joohee) git status
현재 브랜치 joohee
브랜치가 'origin/joohee'에 맞게 업데이트된 상태입니다.

커밋할 사항 없음, 작업 폴더 깨끗함
➜ 문승현 git:(joohee) ls
README.md
➜ 문승현 git:(joohee) cd ..
➜ sesacOS_Study git:(joohee) ls
README.md 문승현 옥주희 이태희 정민희 김율리아
김원석 박보미 이성현 임유빈 정재은
➜ sesacOS_Study git:(joohee) cd 옥주희
➜ 옥주희 git:(joohee) ls
README.md
➜ 옥주희 git:(joohee) cat README.md
test...
최신 버전의 git
git pull -> add -> commit -> push
➜ 옥주희 git:(joohee) vim README.md
➜ 옥주희 git:(joohee) ✗ git status
현재 브랜치 joohee
브랜치가 'origin/joohee'에 맞게 업데이트된 상태입니다.

커밋하도록 정하지 않은 변경 사항:
(무엇을 커밋할지 바꾸려면 "git add <파일>..."을 사용하십시오)
(use "git restore <file>..." to discard changes in working directory)
수정함: README.md

커밋할 변경 사항을 추가하지 않았습니다 ("git add" 및/또는 "git commit -a"를
사용하십시오)
➜ 옥주희 git:(joohee) ✗ git add .
➜ 옥주희 git:(joohee) ✗ git commit -m 'new branch'
[joohee 163c267] new branch
1 file changed, 2 insertions(+)
➜ 옥주희 git:(joohee) git push
오브젝트 나열하는 중: 7, 완료.
오브젝트 개수 세는 중: 100% (7/7), 완료.
Delta compression using up to 6 threads
오브젝트 압축하는 중: 100% (3/3), 완료.
오브젝트 쓰는 중: 100% (4/4), 396 bytes | 396.00 KiB/s, 완료.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/sesacOS/sesacOS_Study.git
3b1547f..163c267 joohee -> joohee
➜ 옥주희 git:(joohee) git remote -v
origin https://github.com/sesacOS/sesacOS_Study.git (fetch)
origin https://github.com/sesacOS/sesacOS_Study.git (push)
➜ 옥주희 git:(joohee) git branch -v

- joohee 163c267 new branch
  main ba73497 Merge pull request #12 from sesacOS/seunghyun
  ➜ 옥주희 git:(joohee) git checkout main  
  'main' 브랜치로 전환합니다
  브랜치가 'origin/main'에 맞게 업데이트된 상태입니다.
  ➜ 옥주희 git:(main) git branch 0v
  ➜ 옥주희 git:(main) git branch -v
  0v ba73497 Merge pull request #12 from sesacOS/seunghyun
  joohee 163c267 new branch
- main ba73497 Merge pull request #12 from sesacOS/seunghyun
  ➜ 옥주희 git:(main) git switch joohee
  'joohee' 브랜치로 전환합니다
  브랜치가 'origin/joohee'에 맞게 업데이트된 상태입니다.
  ➜ 옥주희 git:(joohee) ✗ git add .
  ➜ 옥주희 git:(joohee) ✗ git commit -m"git md"
  [joohee 63398bb] git md
  1 file changed, 487 insertions(+)
  create mode 100644 "\354\230\245\354\243\274\355\235\254/git.md"
  ➜ 옥주희 git:(joohee) git push origin main
  Everything up-to-date
  ➜ 옥주희 git:(joohee) ls  
  README.md git.md
  ➜ 옥주희 git:(joohee) git add git.md
  ➜ 옥주희 git:(joohee) git commit -m "add git.md"
  현재 브랜치 joohee
  브랜치가 'origin/joohee'보다 1개 커밋만큼 앞에 있습니다.
  (로컬에 있는 커밋을 제출하려면 "git push"를 사용하십시오)

커밋할 사항 없음, 작업 폴더 깨끗함
➜ 옥주희 git:(joohee) git status
현재 브랜치 joohee
브랜치가 'origin/joohee'보다 1개 커밋만큼 앞에 있습니다.
(로컬에 있는 커밋을 제출하려면 "git push"를 사용하십시오)

커밋할 사항 없음, 작업 폴더 깨끗함
➜ 옥주희 git:(joohee) git log
commit 63398bbf4346c4d06c743d323933741c2fd26f61 (HEAD -> joohee)
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 19:06:06 2022 +0900

    git md

commit 163c2679365e15914e89feb789f39b6487e10cb4 (origin/joohee)
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 18:58:46 2022 +0900

    new branch

commit 3b1547fca345670b2f371f1b38ac29d9c8e171a8
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 18:37:12 2022 +0900

    new branch

commit e019a4ddbeed61a3e03c3b45bb2e1fcc405bd269
Author: Harimad <leesh68481@gmail.com>
Date: Tue Oct 25 18:21:25 2022 +0900

    add 1 person

commit 66b1920aef723a01bf129bb59870fb9e42667f57
Merge: bc28c11 059af82
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Tue Oct 25 17:42:19 2022 +0900

    Merge pull request #4 from sesacOS/yuuulya

    [YUL] week-1 note upload

commit 059af827eea0ff4807a1c65a0406decef1848fcd (origin/yuuulya)
Author: yuuulya <yla101@naver.com>
Date: Tue Oct 25 17:41:15 2022 +0900

    [YUL] week-1 note upload

commit bc28c117bae3645c1457fc5031218d1b3cd08b89
Merge: 8abfe7e 4bbe657
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:41:18 2022 +0900

    Merge pull request #3 from sesacOS/seongHyeon

    test5

commit 4bbe657819fb13d53037e530c5cfd058d933c6cf (origin/seongHyeon)
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:37:31 2022 +0900

    test5

commit 8abfe7eb1dd23c84137b66be8be83b89b3b3debe
Merge: ec149b6 98d320d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:08:48 2022 +0900

    Merge pull request #2 from sesacOS/seongHyeon

    SH test4

commit 98d320dddbdb3abb58207414f0a883a3bffc68f2
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:06:37 2022 +0900

    SH test4

commit ec149b628354982af299209a7743065c8219f675
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 19:44:03 2022 +0900

    test3

commit 16fca52e013b89b566734e4b5d9b425e518adb61
Merge: e6c4e39 061641c
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Mon Oct 24 19:41:58 2022 +0900

    Merge pull request #1 from sesacOS/yuuulya

    github upload test

commit 061641c4d4533b5c9dacd9a2fbf546084883d0ca
Author: yuuulya <yla101@naver.com>
Date: Mon Oct 24 19:22:51 2022 +0900

    github upload test

commit e6c4e3959ed05213b56594f50ec2b7bc73b7897b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:46:27 2022 +0900

    join 1 people

commit fc0d21785f94ae123cf8fc17eb25b91ee6947bea
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:43:59 2022 +0900

    test2

commit 4bcfa3ad2a627d98625a7826a155d592b5764da3
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:37:22 2022 +0900

    joined 2 people

commit 9aff9ae68bb692fa240f3d199bba0b658ca33846
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:23:11 2022 +0900

    [SH] test

commit 690ca5d29a8ed0308d7158da24dfe8e9ccad59ca
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:21:23 2022 +0900

    Update README.md

commit f096b5c83ac48284ce99383647520a13dd59531d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:00:14 2022 +0900

    Update README.md

commit ba666507be258339b4e5945edbab74bd46a3342b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:12:04 2022 +0900

    made folders & files

commit a085e582a959c0e05e0e815c2ffaa8e8af1c4410
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:03:29 2022 +0900

    Initial commit

➜ 옥주희 git:(joohee) git status
현재 브랜치 joohee
브랜치가 'origin/joohee'보다 1개 커밋만큼 앞에 있습니다.
(로컬에 있는 커밋을 제출하려면 "git push"를 사용하십시오)

커밋할 사항 없음, 작업 폴더 깨끗함
➜ 옥주희 git:(joohee) git commit git.md
현재 브랜치 joohee
브랜치가 'origin/joohee'보다 1개 커밋만큼 앞에 있습니다.
(로컬에 있는 커밋을 제출하려면 "git push"를 사용하십시오)

커밋할 사항 없음, 작업 폴더 깨끗함
➜ 옥주희 git:(joohee) git log
commit 63398bbf4346c4d06c743d323933741c2fd26f61 (HEAD -> joohee)
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 19:06:06 2022 +0900

    git md

commit 163c2679365e15914e89feb789f39b6487e10cb4 (origin/joohee)
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 18:58:46 2022 +0900

    new branch

commit 3b1547fca345670b2f371f1b38ac29d9c8e171a8
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 18:37:12 2022 +0900

    new branch

commit e019a4ddbeed61a3e03c3b45bb2e1fcc405bd269
Author: Harimad <leesh68481@gmail.com>
Date: Tue Oct 25 18:21:25 2022 +0900

    add 1 person

commit 66b1920aef723a01bf129bb59870fb9e42667f57
Merge: bc28c11 059af82
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Tue Oct 25 17:42:19 2022 +0900

    Merge pull request #4 from sesacOS/yuuulya

    [YUL] week-1 note upload

commit 059af827eea0ff4807a1c65a0406decef1848fcd (origin/yuuulya)
Author: yuuulya <yla101@naver.com>
Date: Tue Oct 25 17:41:15 2022 +0900

    [YUL] week-1 note upload

commit bc28c117bae3645c1457fc5031218d1b3cd08b89
Merge: 8abfe7e 4bbe657
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:41:18 2022 +0900

    Merge pull request #3 from sesacOS/seongHyeon

    test5

commit 4bbe657819fb13d53037e530c5cfd058d933c6cf (origin/seongHyeon)
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:37:31 2022 +0900

    test5

commit 8abfe7eb1dd23c84137b66be8be83b89b3b3debe
Merge: ec149b6 98d320d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:08:48 2022 +0900

    Merge pull request #2 from sesacOS/seongHyeon

    SH test4

commit 98d320dddbdb3abb58207414f0a883a3bffc68f2
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:06:37 2022 +0900

    SH test4

commit ec149b628354982af299209a7743065c8219f675
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 19:44:03 2022 +0900

    test3

commit 16fca52e013b89b566734e4b5d9b425e518adb61
Merge: e6c4e39 061641c
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Mon Oct 24 19:41:58 2022 +0900

    Merge pull request #1 from sesacOS/yuuulya

    github upload test

commit 061641c4d4533b5c9dacd9a2fbf546084883d0ca
Author: yuuulya <yla101@naver.com>
Date: Mon Oct 24 19:22:51 2022 +0900

    github upload test

commit e6c4e3959ed05213b56594f50ec2b7bc73b7897b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:46:27 2022 +0900

    join 1 people

commit fc0d21785f94ae123cf8fc17eb25b91ee6947bea
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:43:59 2022 +0900

    test2

commit 4bcfa3ad2a627d98625a7826a155d592b5764da3
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:37:22 2022 +0900

    joined 2 people

commit 9aff9ae68bb692fa240f3d199bba0b658ca33846
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:23:11 2022 +0900

    [SH] test

commit 690ca5d29a8ed0308d7158da24dfe8e9ccad59ca
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:21:23 2022 +0900

    Update README.md

commit f096b5c83ac48284ce99383647520a13dd59531d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:00:14 2022 +0900

    Update README.md

commit ba666507be258339b4e5945edbab74bd46a3342b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:12:04 2022 +0900

    made folders & files

commit a085e582a959c0e05e0e815c2ffaa8e8af1c4410
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:03:29 2022 +0900

    Initial commit

➜ 옥주희 git:(joohee) git status
현재 브랜치 joohee
브랜치가 'origin/joohee'보다 1개 커밋만큼 앞에 있습니다.
(로컬에 있는 커밋을 제출하려면 "git push"를 사용하십시오)

커밋할 사항 없음, 작업 폴더 깨끗함
➜ 옥주희 git:(joohee) git branch 0v
fatal: a branch named '0v' already exists
➜ 옥주희 git:(joohee) git branch -v
0v ba73497 Merge pull request #12 from sesacOS/seunghyun

- joohee 63398bb [1개 앞] git md
  main ba73497 Merge pull request #12 from sesacOS/seunghyun
  ➜ 옥주희 git:(joohee) git checkout main
  'main' 브랜치로 전환합니다
  브랜치가 'origin/main'에 맞게 업데이트된 상태입니다.
  ➜ 옥주희 git:(main) git branch -v
  0v ba73497 Merge pull request #12 from sesacOS/seunghyun
  joohee 63398bb [1개 앞] git md
- main ba73497 Merge pull request #12 from sesacOS/seunghyun
  ➜ 옥주희 git:(main) git status
  현재 브랜치 main
  브랜치가 'origin/main'에 맞게 업데이트된 상태입니다.

추적하지 않는 파일:
(커밋할 사항에 포함하려면 "git add <파일>..."을 사용하십시오)
git.md

커밋할 사항을 추가하지 않았지만 추적하지 않는 파일이 있습니다 (추적하려면 "git
add"를 사용하십시오)
➜ 옥주희 git:(main) ✗ git add .
➜ 옥주희 git:(main) ✗ git commit -m "add git.md"
[main 7a6a4ae] add git.md
1 file changed, 487 insertions(+)
create mode 100644 "\354\230\245\354\243\274\355\235\254/git.md"
➜ 옥주희 git:(main) git push -u origin main
오브젝트 나열하는 중: 6, 완료.
오브젝트 개수 세는 중: 100% (6/6), 완료.
Delta compression using up to 6 threads
오브젝트 압축하는 중: 100% (4/4), 완료.
오브젝트 쓰는 중: 100% (4/4), 4.74 KiB | 4.74 MiB/s, 완료.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/sesacOS/sesacOS_Study.git
ba73497..7a6a4ae main -> main
branch 'main' set up to track 'origin/main'.
➜ 옥주희 git:(main) git log
commit 7a6a4ae1e7cf2492491b18148fe12ac77f0dad2a (HEAD -> main, origin/main, origin/HEAD)
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 19:10:57 2022 +0900

    add git.md

commit ba734978457fdbc081e573ec877ec5b86c90533d (0v)
Merge: 4342ac5 fc5c7db
Author: anstmdgus <47172522+anstmdgus@users.noreply.github.com>
Date: Tue Oct 25 18:50:20 2022 +0900

    Merge pull request #12 from sesacOS/seunghyun

    승현 update

commit fc5c7dbdc9d6873dd0a074a9aef9b46fd22a26a9
Author: moon <anstmdgus473@naver.com>
Date: Tue Oct 25 18:49:28 2022 +0900

    승현 update

commit 4342ac5bd56ace7e8018881425fb3ca25e444227
Merge: a925e1d c7d85da
Author: Been0701 <108451986+Been0701@users.noreply.github.com>
Date: Tue Oct 25 18:48:37 2022 +0900

    Merge pull request #11 from sesacOS/yubeen

    수정 후 커밋

commit a925e1d6b966efe913fd15ae8f1e9e3501513311
Merge: 5307536 068a3b6
Author: taehee <113709273+taeheehi@users.noreply.github.com>
Date: Tue Oct 25 18:46:44 2022 +0900

    Merge pull request #9 from sesacOS/taehee

    hello.html upload

commit 530753648b460d9c21c15608b5168bb265eb99b7
Merge: 1f50a6d 3b1547f
Author: jooheeok <65056196+jooheeOk@users.noreply.github.com>
Date: Tue Oct 25 18:46:27 2022 +0900

    Merge pull request #10 from sesacOS/joohee

    new branch

commit 1f50a6d5b4325e4c340e5f75540be97ae37657a5
Merge: 8690aa9 9ad98fb
Author: sognociel <110799821+sognociel@users.noreply.github.com>
Date: Tue Oct 25 18:45:46 2022 +0900

    Merge pull request #8 from sesacOS/bomi

    test

commit c7d85da08fc27c6f7dab57c78859daf2cbc5b400
Author: Been0701 <dlwptlwkr93@naver.com>
Date: Tue Oct 25 18:45:39 2022 +0900

    수정 후 커밋

commit 068a3b6f6fc31ac3833905c0360af448eda03c50
Author: DESKTOP-O4MJ0GF\LGE <taehi.dev@gmail.com>
Date: Tue Oct 25 18:43:22 2022 +0900

    hello.html upload

commit 8690aa961854f84381dd71844a2cb79452ce5a36
Merge: 3267f04 f0b427d
Author: jeongminhui <62429295+jeongminhui@users.noreply.github.com>
Date: Tue Oct 25 18:41:32 2022 +0900

    Merge pull request #7 from sesacOS/minhee

    upload tes

commit 9ad98fb88901438f195131c7dc6479e34517b952
Author: sognociel <sognociel@gmail.com>
Date: Tue Oct 25 18:40:23 2022 +0900

    test

commit 3267f04d9dfae101f9a26d954eb55c34cee5a246
Merge: 636925d 6390c77
Author: Been0701 <108451986+Been0701@users.noreply.github.com>
Date: Tue Oct 25 18:39:42 2022 +0900

    Merge pull request #6 from sesacOS/yubeen

    first commit

commit 636925d7e7a3662be491aa42b84f12e636f2cd5d
Merge: e019a4d 4666e3f
Author: may-jan <116541435+may-jan@users.noreply.github.com>
Date: Tue Oct 25 18:39:15 2022 +0900

    Merge pull request #5 from sesacOS/jaeeun

    first commit

commit f0b427d383410a3be15b1491b8ad57af4b547fca (origin/minhee)
Author: DESKTOP-881NP36\minhee <jeongminhui0503@gmail.com>
Date: Tue Oct 25 18:38:54 2022 +0900

    upload tes

commit 6390c774f1bc6b9dedcd42f1e0bcddfdc37b18df
Author: Been0701 <dlwptlwkr93@naver.com>
Date: Tue Oct 25 18:38:30 2022 +0900

    first commit

commit 4666e3f97932d7e1bceb9067cde4dc4fbaae104f
Author: jaeeun <jaeeun9862@gmail.com>
Date: Tue Oct 25 18:38:03 2022 +0900

    first commit

commit 3b1547fca345670b2f371f1b38ac29d9c8e171a8
Author: joohee Ok <jooheeok92@gmail.com>
Date: Tue Oct 25 18:37:12 2022 +0900

    new branch

commit e019a4ddbeed61a3e03c3b45bb2e1fcc405bd269
Author: Harimad <leesh68481@gmail.com>
Date: Tue Oct 25 18:21:25 2022 +0900

    add 1 person

commit 66b1920aef723a01bf129bb59870fb9e42667f57
Merge: bc28c11 059af82
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Tue Oct 25 17:42:19 2022 +0900

    Merge pull request #4 from sesacOS/yuuulya

    [YUL] week-1 note upload

commit 059af827eea0ff4807a1c65a0406decef1848fcd (origin/yuuulya)
Author: yuuulya <yla101@naver.com>
Date: Tue Oct 25 17:41:15 2022 +0900

    [YUL] week-1 note upload

commit bc28c117bae3645c1457fc5031218d1b3cd08b89
Merge: 8abfe7e 4bbe657
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:41:18 2022 +0900

    Merge pull request #3 from sesacOS/seongHyeon

    test5

commit 4bbe657819fb13d53037e530c5cfd058d933c6cf (origin/seongHyeon)
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:37:31 2022 +0900

    test5

commit 8abfe7eb1dd23c84137b66be8be83b89b3b3debe
Merge: ec149b6 98d320d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:08:48 2022 +0900

    Merge pull request #2 from sesacOS/seongHyeon

    SH test4

commit 98d320dddbdb3abb58207414f0a883a3bffc68f2
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 20:06:37 2022 +0900

    SH test4

commit ec149b628354982af299209a7743065c8219f675
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 19:44:03 2022 +0900

    test3

commit 16fca52e013b89b566734e4b5d9b425e518adb61
Merge: e6c4e39 061641c
Author: yuuulya <95074363+yuuulya@users.noreply.github.com>
Date: Mon Oct 24 19:41:58 2022 +0900

    Merge pull request #1 from sesacOS/yuuulya

    github upload test

commit 061641c4d4533b5c9dacd9a2fbf546084883d0ca
Author: yuuulya <yla101@naver.com>
Date: Mon Oct 24 19:22:51 2022 +0900

    github upload test

commit e6c4e3959ed05213b56594f50ec2b7bc73b7897b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:46:27 2022 +0900

    join 1 people

commit fc0d21785f94ae123cf8fc17eb25b91ee6947bea
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:43:59 2022 +0900

    test2

commit 4bcfa3ad2a627d98625a7826a155d592b5764da3
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 13:37:22 2022 +0900

    joined 2 people

commit 9aff9ae68bb692fa240f3d199bba0b658ca33846
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:23:11 2022 +0900

    [SH] test

commit 690ca5d29a8ed0308d7158da24dfe8e9ccad59ca
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:21:23 2022 +0900

    Update README.md

commit f096b5c83ac48284ce99383647520a13dd59531d
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 11:00:14 2022 +0900

    Update README.md

commit ba666507be258339b4e5945edbab74bd46a3342b
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:12:04 2022 +0900

    made folders & files

commit a085e582a959c0e05e0e815c2ffaa8e8af1c4410
Author: Harimad <leesh68481@gmail.com>
Date: Mon Oct 24 10:03:29 2022 +0900

    Initial commit

➜ 옥주희 git:(main) git remote add me https://github.com/sesacOS/sesacOS_Study.git
➜ 옥주희 git:(main) git remote -v
me https://github.com/sesacOS/sesacOS_Study.git (fetch)
me https://github.com/sesacOS/sesacOS_Study.git (push)
origin https://github.com/sesacOS/sesacOS_Study.git (fetch)
origin https://github.com/sesacOS/sesacOS_Study.git (push)
➜ 옥주희 git:(main)

공동작업을 했을 때

저장소 확인하는 법 -> git remote -v
브랜치 확인하는 법 -> git branch -v
브랜치 바꾸는 법 -> git checkout (브랜치)
저장소를 생성하는 법 -> git remote add (저장소명) (git 주소)

git pull origin(저장소) main(브랜치)
git status
1.html 2.html
git add file

ls
1.html 2.html
git add 1.html
git commit -m "add 1.html"
git add 2.html
git commit -m "add 2.html"

git status
커밋할 상황이 없습니;다.

git push origin(저장소) main(브랜치)

git push origin(저장소) me(브랜치)

main 권한 가진 사람이 me에 올린 내용을 pull request로 승인해줌
-> main 브랜치에 합쳐짐

git add .
git commit
git push origin main
