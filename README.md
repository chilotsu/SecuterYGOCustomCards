# SecuterYGOCustomCards
Cards preview : https://www.ygopro.co/Forum/tabid/95/g/posts/t/49230/Secuter-custom-cards-for-EDOPro

### Downloads
zip with cards for EDOPro : https://drive.google.com/file/d/1XMfXm4gN0MUpIKkFSwr6Fos4FP3CeQl1/view?usp=sharing
 
strings.conf file : https://drive.google.com/file/d/1veZA7dNbbDxV6sJXJqtuhn4JkzM5jHpr/view?usp=sharing

MSE : https://drive.google.com/file/d/1Ud7nordPqC3zbp7vqgUKH45VW-HymRzm/view?usp=sharing


# Autosync with Github

You can also edit your config.json file in EDOPro to automatically download the new cards from this repository to EDOPro! It's located in the ProjectIgnis\config folder.

The config.json is structured this
{
	"repos": [
   ...
 ],
	"urls": [
   ...
 ],
 ...

You need to add this to 'repos' to download card data and scripts.
		{
			"url": "https://github.com/Secuter/SecuterYGOCustomCards",
			"repo_name": "Secuter Custom Cards",
			"repo_path": "./repositories/secuter-custom-cards",
			"data_path": "expansions",
			"script_path": "script",
			"should_update": true,
			"should_read": true
		}

And these in 'urls' to download card images.
		{
			"url": "https://raw.githubusercontent.com/Secuter/SecuterYGOCustomCards-pics/master/{}.png",
			"type": "pic"
		},
		{
			"url": "https://raw.githubusercontent.com/Secuter/SecuterYGOCustomCards-pics/master/field/{}.png",
			"type": "field"
		}

PS: Images are not updated if there is a change in the card, you have to manually delete the old image to automatically download the new one.
