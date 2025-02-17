---
# required metadata

title: Add or remove a label to or from an Azure Information Protection policy - AIP
description: Add or remove an Azure Information Protection label to or from the global policy for all users, or to or from a scoped policy for a subset of users.
author: cabailey
ms.author: cabailey
manager: barbkess
ms.date: 07/17/2019
ms.topic: conceptual
ms.collection: M365-security-compliance
ms.service: information-protection
ms.assetid: 0546cc11-67a5-4194-8c54-f3ac8ce9ebe1

# optional metadata


#ROBOTS:
#audience:
#ms.devlang:
ms.subservice: aiplabels
#ms.reviewer: eymanor
#ms.suite: ems
#ms.tgt_pltfrm:
ms.custom: admin

---

# Add or remove a label to or from an Azure Information Protection policy

>*Applies to: [Azure Information Protection](https://azure.microsoft.com/pricing/details/information-protection)*
>
> *Instructions for: [Azure Information Protection client for Windows](faqs.md#whats-the-difference-between-the-azure-information-protection-client-and-the-azure-information-protection-unified-labeling-client)*

After you create an Azure Information Protection label, you can then add it to a policy so that it is available for users. If the label is for all users, add the label to the global policy. If the label is for a subset of users, add the label to a scoped policy. A label can be added to only one policy. 

To add a sublabel, its parent label must be in the same policy, or in the global policy. When you add a sublabel, settings from the main label are not inherited. For users who are assigned the sublabel in their policy, the main label is supported only as a display container for the name and color. In this scenario, other configuration settings in the main label are not supported for visual markings, protection, and conditions. Although you can still configure them, those settings in the main label are supported only for users who have the main label in their policy without the sublabel.

For labels that are already in a policy, you can remove them from the policy. This action does not delete the label. It remains available to be used in another policy.

If you haven't yet created the label, see [How to create a new label for Azure Information Protection](configure-policy-new-label.md).

If you need to create a scoped policy so that the label applies to a subset of users, see [How to configure the Azure Information Protection policy for specific users by using scoped policies](configure-policy-scope.md).

## To add or remove a label to or from a policy

1. If you haven't already done so, open a new browser window and [sign in to the Azure portal](configure-policy.md#signing-in-to-the-azure-portal). Then navigate to the **Azure Information Protection** blade.
    
    For example, on the hub menu, click **All services** and start typing **Information** in the Filter box. Select **Azure Information Protection**.

2. From the **Classifications** > **Policies** menu option: On the **Azure Information Protection** - **Policies** blade, select **Global** if the label to add or remove applies to all users.

    If the label to add or remove applies to a subset of users, select your scoped policy instead.

3. On the **Policy** blade, select **Add or remove labels**.

4. On the **Policy: Add or remove labels** blade, you see all your labels with a checkbox selected if they are already in a policy, and the corresponding policy name in the **POLICY** column.
     
    Sublabels display as indented. In a scoped policy, labels that are inherited from the global policy display as unavailable.
    
    Do one or more of the following actions, and then click **OK**:
    
    - To add a label, select it, which adds a selected checkbox.
    
    - To remove a label, clear its checkbox.
  
5. To save your changes, click **Save**.
   
    Your changes are automatically available to users and services. There's no longer a separate publish option.


## Next steps

For more information about configuring your Azure Information Protection policy, use the links in the [Configuring your organization's policy](configure-policy.md#configuring-your-organizations-policy) section.
