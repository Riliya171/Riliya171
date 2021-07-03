import discord
from discord import colour
from discord import embeds
from discord import client
from discord.ext import commands
from discord.ext import tasks
from asyncio import *
import random
from discord.ext.commands.core import command
from discord.ext.commands.errors import DisabledCommand
client = commands.Bot(command_prefix = ".")
client.remove_command("help")
Token = "ODYwOTA5MTgxNzYyMDExMTg3.YOCGJw.GHAieRuy9tsB_rW477OfrbA4PlA"

@client.event
async def on_ready():
    await client.change_presence(status = discord.Status.do_not_disturb)

@client.command()
async def سلام(j2):
    await j2.send("سلام بابات چطوره")
    @client.command()
async def بای(j2):
    await j2.send("برو دیگه بر نگردی")
    @client.command()
async def گوه (j2):
    await j2.send("اسم خانوادت رو نیمخواد ببری")
    @client.command()
async def چطوری(j2):
    await j2.send("خوبم تو چطوری موتوری :D")
client.run("ODYwOTA5MTgxNzYyMDExMTg3.YOCGJw.GHAieRuy9tsB_rW477OfrbA4PlA")
