# Integration: Google Api OAuth 2.0 from Salesforce

####Steps to Follow:
1. Add remote site settings
2. Create custom metadata for storing access token and endpoints 
3. Create a vf page and use that as redirect uri
4. Create a custom label to store master label of custom metadata record
5. Prepare the url to get authorization code
6. Develop an apex class to get access token and deploy to custom mtd
7. Implement refresh_token after access_token expired

#### It is a Framework to Integrate any OAuth2.0 from salesforce


#####Note:
1. To enable SSO login in salesforce follow:
My Domain -> Authentication Configuration -> Enable Google, Slack or Facebook Option (Auth provider setup required)
2. No need to use remote site settings and refresh for named credentials, it will take care.
3. Add Callback Url from Salesforce Auth Provider as another redirect_uri in connected app of other platform (refresh_token problem solved)
4. In Named Credential add openid along with other scopes
