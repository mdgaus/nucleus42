# Nucleus42 Front End 

## The project includes Modules/Components/Template/Style
   the project nclient folder contains the following 

### Modules

   1. Companies Search Page   
   2. Investors Search Page   
   3. Company Profile Form Edit  
   4. Person Profile Form Edit   
   5. BubbleChart on Profile Page   
   
### Components

   all the reactjs components are under /public/javascripts/app/components/   
   Company: company search page contains multiple components with filters, companies list and options to select more columns  
   Investor: investor search page contains multiple components with filters, investors list and options to select more columns 
   Person: person profile edit contains multiple forms sections with card layout and dropdowns
   Graph/BubbleChart.js: used to display investments sectors, common to company/person profile  
   ContactInfoForm.js: reusable form for social links section, common to Company/Person profile edit  
   CustomizeDropDown.js: reusable drop down to use company type and team size for company profile edit   
   EditComp.js: company profile edit contains multiple forms sections with card layout, tags and dropdowns  
   EditCompGeneral.js: general information section on company profile edit 
   EditPersonRolesDropDown.js:   
   FundingInvestmentForm.js: reusable form used for Angel investment, Funding and Portfolio. common to Company/Person profile edit  
   SuggestionsDropdownClaim.js: reusable dropdown comes with backend-API data, common to all sections of Company/Person profile edit   
   SuggestionTag.js: reusable component used for displaying text in tags common to all sections of Company/Person profile edit   
   TeamProfile.js: reusable form for Team section on Company profile edit, common to all team sections   
   utils.js: contains reusable blocks of code such as error notification, convert date format, experiences/team member card layout and static JSON data, common to all    
   
### Template

   all the view pages for initial rendering are under view folder
   ejs template contains html or html and JSX 
   source: /views/
   index.ejs:  
   companies.ejs:    
   company-profile-edit.ejs:   
   footerNew.ejs:    
   investors.ejs:    
   navbar-new.ejs:   
   person-profile-edit.ejs:   
   signupform.ejs:   
   
### Styling

   all the styling files are under /public/stylesheets/sass/
   
   
## The project removes unnecessary files
   the project nclient folder contains the following 
   
### Components

   source: /public/javascripts/app/components/
   ClaimButton.js     
   CompanyType.js     
   EditCompFounder.js    
   EditCompFunding.js    
   EditPortfolio.js      
   EditProfileCalendar.js   
   Investors.js    
  
   source: /public/javascripts/app/components/Person/     
   CompanyRole.js  
   source: /public/javascripts/app/components/Utility/    
   ClaimProfileButton.js    
  
### Templates

   source: /views/ 

   claimprofile.ejs   
   company-profile-new.ejs  
   footer.ejs   
   navbar.ejs   
   portfolio_view_all_section.ejs    
   tags_section.ejs   
  
### Styling

   source: /public/stylesheets/sass/    

   _footer.scss    
   _nav.scss    
   _right-tag.scss    
  
