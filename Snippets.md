# Snippets

## **fatal: remote origin already exists**
---

### *URL:*

https://tinyurl.com/2mvuor8w

### *Explanation:*

``remote`` refers to the hosted repository. ``origin`` is the pointer to where that ``remote`` is. Most of the time, ``origin`` is the only pointer there is on a local repository.

If you want to change the pointing URL attached to ``origin``, you can remove the existing ``origin`` and then add it back in again with the correct URL.
To remove your handler, use the remove command on ``remote``, followed by the handler name – which, in our case, is ``origin``.

### *Snippet:*

    git remote remove origin

---

## **Save SSH key phrase**

### *URL:*

https://stackoverflow.com/a/10032655/13278191

### *Explanation:*

The ssh key is not added to the project, therefore the ssh key-phrase has to be entered every time.
Save the ssh key via the ssh agent, make life more convenient

### *Snippet:*

Start ssh agent

    eval $(ssh-agent)

Add private key

    ssh-add

---