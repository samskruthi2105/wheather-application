
git checkout -b dev


git checkout -b feature-ui


echo "UI change" >> file.txt
git add file.txt
git commit -m "UI change"


git checkout dev
echo "Dev change" >> file.txt
git add file.txt
git commit -m "Dev change"


git merge feature-ui
git add file.txt
git commit -m "Resolved merge conflict"

