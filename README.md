# Spotify.me

Use Ajax to load data from the Spotify API! A user should be able to:

**Basic Requirements:**

 - Enter a keyword to seach for and.
 - Select "album", "artist", or "track" as the search type.
 - Have the names of all search results print as a list.
 - When the user changes the search type selector, reload the results list based on the new search type.
 
**Keep going:**

 - Add a "Showing X-X of X results found" message.
 - Setup pagination links for accessing the next page of results.
 
 
 **Use the Spotify API**  
 
[Spotify API](https://developer.spotify.com/web-api/search-item/)


### Git Branching.

This will be completed by a Team. Each member of the team will be repsonsible for one task. Possibly, 

1. Search by album.  
2. Search by artist.  
3. Search by track.  

#### Procedure
* One team member will fork this repo that the team will share.
	* Can use any team member's github account to hold this forked repo.
	* Add other team members as colloborators to this repo. 
		 _See the Setting on the right in the github repo_.  
* Each team member clones repo on thier local machine.  
* Each team member creates a _topic_ branch for their task.  
	 This branch should also have a remote branch, _tracking branch in the github repo_.
	 
	 ```
	 	git checkout -b <topic/feature branch name>
	 	git push origin <topic/feature branch name>
	 ```
	 
* Each team member will periodically update their master branch and rebase their topic branch from the master branch.

	```
		git checkout master
		git pull origin master
		git checkout <topic/feature branch name>
		git rebase master
		# May have to resolve merge conflicts. But, probably will not.
	```
	
	Now the feature branch is up to date with master.  
	
* When the feature is complete the feature _owner_ will merge the topic/feature branch into the master and push up to github.  

	```
		git checkout master
		git merge <topic/feature branch name>
		git push origin master
	```

