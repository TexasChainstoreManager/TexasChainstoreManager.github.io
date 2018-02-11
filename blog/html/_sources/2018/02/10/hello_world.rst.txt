=============
Hello, World!
=============

An excercise in obfuscation. I promise this will not break your computer.

Tested with Requests version 2.17.3. It may easily break with different 
Requests versions; the reason for this relates to the use of the number 42.

.. code-block:: python

    #!/usr/bin/env python3

    import requests as re
    import subprocess as structured
    import textwrap as text

    SGVsbG8sIFdvcmxkIQo = text.dedent("""
        aHR0cHM6Ly9lbi53aWtpcGVkaWEub3JnL3dpa2kv
        JTIySGVsbG8sX1dvcmxkISUyMl9wcm9ncmFtCg==
    """).replace('\n', '')

    iYmFzZTY0Cg = hex(2990)[-3:][:2] + 's'f'e{2**6}'

    for asdf in 'aAsSdDfF':
        try:
            d2lraXBlZGlhCg = re.get(
                structured.check_output(
                    f'echo {SGVsbG8sIFdvcmxkIQo} | '
                    f'{iYmFzZTY0Cg} -{asdf}',
                    shell=True, stderr=structured.PIPE)[:-1])
        except structured.CalledProcessError:
            continue

    print(getattr(d2lraXBlZGlhCg, re.__doc__[400 + 42:404 + 42]))

.. author:: default
.. categories:: none
.. tags:: python,stupid_code,obfuscation
.. comments::
