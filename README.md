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
   
   ```
   Company:- company search page contains multiple components with filters, companies list and options to select more columns 
         /Company/Companies.js:- renders companies table and filters
         /Company/FundingRange.js:- component used for funding range under Range Filter on companies search page
         /Company/MainSearchBox.js:- reusable search box results drop down for searching startups, investors etc.., common to landing page, navigation bar
         /Company/SelectTags.js:- reusable component for displaying filter text in tags, common to all filters on companies search page
         /Company/SuggestionsDropdown.js:- search box drop down for filters on companies search page
         /Company/YearFounded:- component used for year of found under Range Filter on companies search page
         /Company/YearFunded:- component used for year of funding under Range Filter on companies page
         
   Investor:- investor search page contains multiple components with filters,investors list and options to select more columns 
         /Investor/Investors.js:- renders investors table and filters
         /Investor/SelectTags.js:- reusable component for displaying filter text in tags, common to all filters on investors search page
         /Investor/SuggestionsDropdown.js:- search box drop down for filters on investors search page
         
   Person:- person profile edit contains multiple forms sections with card layout and dropdowns
   
   Graph/BubbleChart.js:- used to display investments sectors, common to company/person profile  
   
   ContactInfoForm.js:- reusable form for social links section, common to Company/Person profile edit  
   
   CustomizeDropDown.js:- reusable drop down to use company type and team size for company profile edit   
   
   EditComp.js:- company profile edit contains multiple forms sections with card layout, tags and dropdowns  
   
   EditCompGeneral.js:- general information section on company profile edit 
   
   EditPersonRolesDropDown.js:- currently using it manually to select type of a company. need to change it later and remove this component when type comes from data. used on Person profile edit
   
   FundingInvestmentForm.js:- reusable form used for Angel investment, Funding and Portfolio. common to Company/Person profile edit  
   
   SuggestionsDropdownClaim.js:- reusable dropdown comes with backend-API data, common to all sections of Company/Person profile edit   
   
   SuggestionTag.js:- reusable component used for displaying text in tags common to all sections of Company/Person profile edit   
   
   TeamProfile.js:- reusable form for Team section on Company profile edit, common to all team sections   
   
   utils.js:- contains reusable blocks of code such as error notification, convert date format, experiences/team member card layout and static JSON data, common to all
```
   
### Template

   all the view pages for initial rendering are under view folder
   
   ejs template contains html or html and JSX 
   
   ```source: /views/
   
   index.ejs: landing/home page 
   companies.ejs:- companies search page and renders component company 
   
   company-profile-edit.ejs:- renders company profile edit component
   
   footerNew.ejs:- footer section
   
   investors.ejs:- investors search page and renders component investor
   
   navbar-new.ejs:- navigation bar with menu items and renders search box drop down component MainSearchBox
   
   person-profile-edit.ejs:- renders person profile edit component
   
   signupform.ejs:- section for email notification subscription on top
```
   
### Styling

   all the styling files are under /public/stylesheets/sass/
   
   
## The project removes unnecessary files

   the project nclient folder contains the following 
   
### Components

   ```source: /public/javascripts/app/components/
   
   ClaimButton.js:- initially this was used for founder to claim founder's profile
   CompanyType.js:- old file that was used to define type and subtype of a company now using EditPersonRolesDropDown
   EditCompFounder.js:- this component is replaced by TeamProfile
   EditCompFunding.js:- this component is replaced by FundingInvestmentForm
   EditPortfolio.js:- this component is replaced by reusable component FundingInvestmentForm
   EditProfileCalendar.js:- this component is replaced by a library react-widget which contains DateTimePicker
   Investors.js:- identical file of investors search page
   
   source: /public/javascripts/app/components/Company/  
   Slider.js:- library for Funding Range slider, not using any slider on companies search page
   
   source: /public/javascripts/app/components/Investor/  
   Slider.js:- library for Funding Range slider, not using any slider on investors search page
   YearFounded:- there is no Range filter to use year of found on investors search page 
   YearFunded:- not using any funding range on investors search page
   
   source: /public/javascripts/app/components/Person/  
   CompanyRole.js:- this was used to select role and subrole for person profile
   
   source: /public/javascripts/app/components/Utility/ 
   ClaimProfileButton.js:- this component is replaced by ClaimBar to claim profile
```
### Templates

   source: /views/ 

   claimprofile.ejs   
   company-profile-new.ejs  
   footer.ejs   
   navbar.ejs   
   portfolio_view_all_section.ejs    
   tags_section.ejs   
  
### Styling

   ```source: /public/stylesheets/sass/    

   _footer.scss    
   _nav.scss    
   _right-tag.scss    
   _slider.scss
  ```
