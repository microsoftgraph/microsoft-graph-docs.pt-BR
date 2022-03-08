---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7879a48f38f56948a1c9d1c9d5a78ac576549d45
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335560"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const crossTenantAccessPolicyConfigurationDefault = {
  b2bCollaborationOutbound: 
  {
    usersAndGroups: 
    {
      accessType: 'blocked',
      targets: [
        {
          target: '0be493dc-cb56-4a53-936f-9cf64410b8b0',
          targetType: 'group'
        }
      ]
    },
    applications: 
    {
      accessType: 'blocked',
      targets: [
        {
          target: 'AllApplications',
          targetType: 'application'
        }
      ]
    }
  }
};

await client.api('/policies/crossTenantAccessPolicy/default')
    .version('beta')
    .update(crossTenantAccessPolicyConfigurationDefault);

```