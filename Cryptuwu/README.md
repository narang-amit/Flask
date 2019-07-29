# Team Nahasapeemapetilon  
### Adil Gondal, Amit Narang, Rubin Peci, & Qian Zhou
   
### Cryptuwu  
   
Cryptuwu is a cryptocurrency forum and market tool.

Users will be able to create accounts to comment on threads relating to all of their cryptocurrency interests, make posts of their own, and upvote other users posts.

#### Features 
- Allows users to make accounts, login, and make posts.
- Posts can be upvoted, saved, and replied to. 
- Stats regarding various crytocurrencies can be viewed, and some coins can be favorited.

### Necessary Packages
1. Datetime   
2. Plotly   
3. Pandas    
4. Passlib    
5. Wheel   
6. Flask    
 
#### How to run the project   
1. Create a virtual environment  
`python -m venv test/`  

2. Activate your virtual environment   
`source test/bin/activate` 
   
3. Clone the repo       
`git clone https://github.com/adil11111/SDFP.git`    

4. Open cloned folder       
`cd SDFP/` 
    
5. Install the necessary python modules   
```
pip3 freeze > requirements.txt
pip3 install -r requirements.txt
``` 
   
6. Procure API keys for the Nomics and Plotly APIs and add them to `keys/(APIname).json`
   
Nomics:  
Get your free API key [here](https://p.nomics.com/cryptocurrency-bitcoin-api)   
Follow the instructions provided, and your API key will be emailed to you.   
Put that API key in the `keys/nomics.json` file, replace the empty string for the entry "API".   
   
Plotly:   
Make an account [here](https://plot.ly/Auth/login/?next=%2Fsettings) and procure your API key.    
Put that API key in the `keys/plotly.json`, replace the empty strings for "username" and "API" with your information. 
 
7. Once the above steps are completed, run the follow command at the root of the repo   
`python app.py`     
*If any errors arise, verify you completed the above steps, and try again. If the error still persists, feel free to open an issue in our repo!*    
    
8. Open your browser, and connect to this [link](http://localhost:5000)   
The link points to localhost:5000, which is the server on which the program is running on your computer   
    
9. Use the site! Make an account, test things out, do as you please.    
   
If you encounter any issues worth noting, open an issue so we can get to it!   
   
Hope you enjoy :blush:  


KNOWN BUGS/ISSUES:   
- API   
	- Nomics API provides faulty data for some dates, making the graph appearing messed up    
	- Plotly only allows 25 graphs per user on the free plan, so one must log in and clear up plots if they have been all used up    
