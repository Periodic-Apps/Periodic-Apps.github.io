---
layout: default
title: Frequently Asked Questions
---

# Frequently Asked Questions

## Who is this app for?

Resourceful is for people of any age who want to change the way Minecraft looks. 

**Parents:** if your kids have been asking you daily to help them make their own “texture pack”, this app is for you. 

**Kids:** if you don’t have access to a PC or lack experience working with all the technologies required to make texture packs, this app is for you.

Even if you don’t own Minecraft, Resourceful is also a fun toy art app. Who doesn’t need more art in their lives?n text goes here

## I just installed the app. Where are all the standard vanilla Minecraft blocks!?

Unfortunately, we cannot distribute the standard Minecraft vanilla textures with the app. The good news is that Mojang provides a default resource pack that you can import into the app. Follow the steps in [How to Import the Vanilla Resource Pack](/how-to-load-the-vanilla-resource-pack) to get this set up.

## Can I share my projects with friends?

Yes! You can share individual projects with friends using the iOS standard share button in the top right corner of the project view. When prompted, tap “Resource Pack (mcpack)” and then using the iOS share sheet, select the person, place, or thing you’d like to send the project to.

## When exporting, what is the difference between a “test world” and “resource pack”?

To make it easy to quickly test your changes, you can export your project as a test world. A test world embeds your resource pack and preloads the player inventory with recently modified blocks.

When you’re ready to share your project with other people, it makes more sense to export just the resource pack so that players can choose which worlds (or servers) to apply the pack to.

## What is the difference between Minecraft and Minecraft RTX?

On some platforms such as Windows 10 (with RTX enabled video cards), Minecraft Bedrock Edition supports a technology called real-time ray tracing which adds a strong element of visual realism to the game. Blocks might appear to glow or have a metallic or polished look. They can also appear bumpy.

Blocks in which you’ve modified the surface properties (i.e. metalness, glow, polish, height) will exhibit those additional qualities on platforms which support RTX.

Learn more about RTX from Mojang and NVIDIA.

## Can I use Resourceful even if I don’t have access to Minecraft RTX?

Yes! Surface properties such as glow, metalness, and polish will be ignored by platforms that don’t support RTX (e.g. Minecraft for iPhone or iPad). Your resource pack will modify the color of blocks which can be transformative nonetheless.

## Does Resourceful support Minecraft Java Edition?

There are no current plans to support Java Edition.

## How do I modify items or mobs?

At this time, Resourceful only supports modifying block textures. We plan to add support for items soon.

The good news is that changing even a few blocks’ textures (e.g. dirt, grass, stone) can dramatically alter the game appearance. And Resourceful makes this really easy to do.

## Why don’t the surface properties such as glow, metal and polish appear in Minecraft?

Minecraft Bedrock Edition only supports these surface properties on platforms which feature RTX. At the time of writing that is only Windows 10. Your texture pack will otherwise still function normally on other platforms and players who do join from a RTX-enabled platform will experience your texture pack in all its glory.

## Why do some textures appear gray such as the top of grass blocks?

Some textures don't have their color added until they're rendered in the game at which point a tint or overlay color is chosen based on the current biome or other factors. One important example of this is the top and sides of Grass blocks. To further complicate matters, tint/overlay colors aren’t always available to Resourceful resulting in some textures appearing in shades of gray in the app. For these textures, it’s best not to add your own color (other than modifying the shades of gray) as Minecraft will ultimately still overlay some other color.

In future versions of the app tint and overlay color will be a configurable property of a texture.

## Where are all the chests?

Some blocks are rendered in Minecraft using a more complex 3D model than the box we all know and love. For instance, Chests, Ender Chests and Trapped Chests are all represented by 3D models that support a latch in the front and a top that flips open. These blocks are not currently supported by Resourceful.

## I erased some pixels and when I reloaded the block those pixels are now black. Why?

On textures which have a masking layer such as grass block or tall grass, it is not possible to erase pixels. Fully and partially transparent pixels lose their transparency when the block is saved. The texture’s alpha channel is reserved for use in controlling the masking layer.

## Can I import 3rd party resource packs?

Resourceful does not officially support 3rd party resource packs although it may work for you under certain circumstances. [Read more here](/importing-3rd-party-resource-packs).

## I modified one block and the changes show up in other blocks. Why?

Within a project (and within an exported resource pack), many blocks share the same underlying textures. For example, Acacia Stairs and Acacia Button use the same texture. This makes it possible to modify a texture once and see the impact consistently across all blocks that use the same texture without needing to manually edit many blocks with the same changes.

In the future, we may introduce a method to break the implicit connection between blocks so that the textures can be independent.

## Some blocks recently added to Minecraft are not present in Resourceful. How do I fix this?

Periodically, Mojang adds new block types to Minecraft. When they do this, they also update the vanilla resource pack you likely installed after first downloading Resourceful. To add any missing blocks to the Vanilla Resource Pack project, repeat the steps in [How to Install the Vanilla Resource Pack](/how-to-load-the-vanilla-resource-pack).

## Where are all the variations of textures?

Many blocks’ textures have more than one texture state. For example, the Wood block comes in a staggering number of varieties: Log Oak, Stripped Oak Log, Log Spruce, Stripped Spruce Log, etc. In Minecraft, we tend to think of these as different blocks. However, in Resourceful (and Bedrock’s modding APIs), all of these states are collapsed to single block with multiple texture states. Another example where texture states crop up is in different ages of the Wheat block which has 8 texture states, one for each of the different ages of wheat.

In all cases, texture states can be accessed while editing an individual texture. For textures that do have multiple states there are three additional buttons located just above the pixel canvas. The left and right arrow buttons make it possible to sequentially traverse the various states. The middle button displays the name of the current texture state. Tapping it brings up a list to select another texture state.

