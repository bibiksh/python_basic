chapter 6: Managing Information
=================================================
이 장에서는 조건문에 대해서 배워 보도록 하자.


6.1 Using if Statements
---------------------------


Mission #26: Blast a Crater
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

다음은 사용자 입력을 받아서 입력 하라고 하면 블력을 생성하는 프로그램이다.

.. code-block:: python


    from mcpi.minecraft import Minecraft
    mc = Minecraft.create()
    answer = input("Create a crater? Y/N ")

    if answer == "Y":
        pos = mc.player.getPos()
        mc.setBlocks(pos.x + 1, pos.y + 1, pos.z + 1, pos.x - 1, pos.y - 1, pos.z - 1, 0)
        mc.postToChat("Boom!")

