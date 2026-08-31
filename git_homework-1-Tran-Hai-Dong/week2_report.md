EXERCISES WEEK2 REPORT


$ git init
git branch -M master
git remote add origin https://github.com/tranhaidong23/git_homework-1-Tran-Hai-Dong.git



PART A:
1. $ echo "file week2.md" > week2.md
   $ git add week2.md
   $ git commit -m " commit cua week2.md"
   $ git checkout -b week2
2.
  $ git commit --allow-empty -m "working 1"
    git commit --allow-empty -m "working 2"

3. 
  $ echo "today is a beautiful day" >> week2,md
  $ git add week2.md
$ git commit -m "Add text line to week2.md"
$ git checkout master
4.
git checkout -b week2b
git merge week2
git branch -d week2

PART B:
1.
git checkout -b wip
echo "noi dung wip" > wip.txt
git add wip.txt
git commit -m "them wip.txt"
2.
git checkout master
git merge week2b
3.
git branch --merged
git branch --no-merged
4.
git branch -d week2b
5.
git branch -m wip work-in-progress
git push -u origin work-in-progress

PART C:
1.
git checkout work-in-progress
echo "update noi dung" >> wip.txt
git add wip.txt
git commit -m "update wip.txt"
2.
$ git branch -vv
3.... on github

PART D:
1.
git checkout master
git checkout -b experiment
echo "exp 1" > exp1.txt && git add exp1.txt && git commit -m "Add exp1.txt"
echo "exp 2" > exp2.txt && git add exp2.txt && git commit -m "Add exp2.txt"
2.
git checkout master
echo "master file" > master_file.txt && git add master_file.txt && git commit -m "Add master file"
3.
git checkout experiment
git rebase master
4.Khi thêm một dòng văn bản vào file week2.md ở nhánh week2 rồi commit lại, dòng văn bản đó chỉ được lưu lại trong lịch sử của riêng nhánh week2.
Khi chuyển về lại nhánh master, mở file week2.md lên sẽ thấy nó không có dòng text mới đó.
5.
git checkout master
git merge experiment
6.push to github
7.Upload report to github
