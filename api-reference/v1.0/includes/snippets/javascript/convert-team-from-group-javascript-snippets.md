---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca5cfb78127a8700592bb852d0183c6aed3b3904b0a3b763f24978eaff947bd1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899222"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   'template@odata.bind':'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')',
   'group@odata.bind':'https://graph.microsoft.com/v1.0/groups(\'dbd8de4f-5d47-48da-87f1-594bed003375\')',
   channels: [
      {
         displayName: 'Class Announcements 📢',
         isFavoriteByDefault: true
      },
      {
         displayName: 'Homework 🏋️',
         isFavoriteByDefault: true
      }
   ],
   memberSettings: {
      allowCreateUpdateChannels: false,
      allowDeleteChannels: false,
      allowAddRemoveApps: false,
      allowCreateUpdateRemoveTabs: false,
      allowCreateUpdateRemoveConnectors: false
   },
   installedApps: [
      {
         'teamsApp@odata.bind':'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'com.microsoft.teamspace.tab.vsts\')'
      },
      {
         'teamsApp@odata.bind':'https://graph.microsoft.com/v1.0/appCatalogs/teamsApps(\'1542629c-01b3-4a6d-8f76-1938b779e48d\')'
      }
   ]
};

await client.api('/teams')
    .post(team);

```