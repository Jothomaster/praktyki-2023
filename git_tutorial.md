# Git tutorial

Git jest narzędziem do łatwego dostępu i edycji plików nie lokalnych. Jednymi z podstawowymi komendami są "git <clone/add/commit/push/pull/checkout> \<dodatkowe parametry>".

Proces robienia i mergowania brancha:
- git checkout [-b] \<nazwa>
- git commit -am "Wiadomość"
- git push origin \<nazwa>
I założyć pull request

W celu uniknięcia merge conflictów dla plików edytowanych przez kilka osób należy poczekać aż inni zpushują zmiany, zpullować i dopiero potem edytować 