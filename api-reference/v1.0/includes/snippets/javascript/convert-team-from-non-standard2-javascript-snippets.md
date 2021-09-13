---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7fabc133a29beaceba386edaa5fa0cd85a73d5ec17a41a51e9ddfe6b1184237d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100761"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   'template@odata.bind':'https://graph.microsoft.com/v1.0/teamsTemplates(\'educationClass\')',
   displayName: 'My Class Team',
   description: 'My Class Team’s Description',
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