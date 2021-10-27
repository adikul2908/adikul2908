- 👋 Hi, I’m @adikul2908
- 👀 I’m interested in ...
- 🌱 I’m currently learning salesforce devlopment
- 💞️ I’m looking to collaborate on salesforce..
- 📫 How to reach me ...

<apex:page controller="visualforceS49" rendered="true" renderAs="pdf">

<apex:form >
<apex:pageBlock title="Vendor Registration Form" rendered="true">
<apex:pageBlockSection title="Company Details"  columns="2">
   

            
                 <apex:outputLabel > Vendor Company Names:  </apex:outputLabel>
          <apex:inputText value="{!ToEntervalue}" id="id1"  onclick="changeCase();" required="True" />   
          
            <apex:outputLabel > Vendor Contact Person:</apex:outputLabel>
            <apex:inputText value="{!VendorContactPerson}" id="id2" rendered="true"/> 
            
            <apex:outputLabel > Amount Per Event:</apex:outputLabel>
            <apex:inputText value="{!PerEvent}" id="id3" rendered="true"/> 
              
            <apex:outputLabel > City:</apex:outputLabel>
            <apex:inputText value="{!Cit}" id="id4" rendered="true"/> 
            
            <apex:outputLabel > Country: </apex:outputLabel>
            <apex:inputText value="{!Count}" id="id5" rendered="true"/> 
            
            <apex:commandButton value="Send Email" onclick="JSFunction('{!$Component.id3}');"/> 
            <apex:commandButton value="Reset"/> 
            <apex:commandButton value="Generate PDF" onclick="Case2('{!$Component.id4}','{!$Component.id5}');" /> 
      
                   </apex:pageBlockSection>
        </apex:pageBlock>    
    </apex:form>
</apex:page>
