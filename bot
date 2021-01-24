@client.command()
@has_permissions(kick_members=True)
async def warn(ctx, user: discord.Member, *, reason):
     warn = discord.Embed(
            description = f"**You have been warned in {ctx.message.guild.name}.** \n \n ```{reason}```  \n \n *To avoid warns make sure you read the server rules. If this warn seems to be incorrect, please appeal with our form link: https://forms.gle/hd8xy5fV2EUtPYks6*",
            colour = discord.Colour.orange())
     await user.send(embed=warn)
if isinstance(discord.ext.commands.errors.CommandInvokeError):
       disable = discord.Embed(
            description = "This user has there DMs disabled. I cannot message them. I have logged there warning instead. \n \n ```py Command raised an exception: Forbidden: 403 Forbidden (error code: 50007): Cannot send messages to this user```",
            colour = discord.Colour.red())
       await ctx.send(embed=disable)
