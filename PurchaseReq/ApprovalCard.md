# Due diligence check
- This is being sent to the KLA HT (@{outputs('Get_user_profile_(V2)_-_KLA_HT')?['body/givenName']} @{outputs('Get_user_profile_(V2)_-_KLA_HT')?['body/surname']}) as you are the Cost Centre Manager for **@{triggerOutputs()?['body/Cost_x0020_Centre/Label']}** and the Office (@{outputs('Get_user_profile_(V2)_-_Nominated_Purchaser')?['body/givenName']} @{outputs('Get_user_profile_(V2)_-_Nominated_Purchaser')?['body/surname']}) will be making the large purchase on your behalf.
- Please check the following items carefully prior to approving the purchase. 
- [View full item](@{triggerOutputs()?['body/{Link}']})

## Item Details
- **Request ID:** @{outputs('Update_item')?['body/RequestID']}
- **Supplier:** @{triggerOutputs()?['body/Supplier/Value']}
- **Item Name:** @{triggerOutputs()?['body/Title']}

## Cost
For further details, [view the full item](@{triggerOutputs()?['body/{Link}']})

- **Grand Total:** @{body('Format_number_-_Grand_Total')}

