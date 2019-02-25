chapter 5: Storing and Modifying Information
===============================================================


5.1 Boolean Basics
----------------------------
A Boolean is a bit like a light switch: it is either True (on) or False (off)


Mission #17: Stop Smashing Blocks!
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

마인크래프트에서 immutable 설정을 on으로 하는 프로그램을 실행해 봅시다.

.. code-block:: python

    from mcpi.minecraft import Minecraft
    mc = Minecraft.create()

    mc.setting("world_immutable", True)


