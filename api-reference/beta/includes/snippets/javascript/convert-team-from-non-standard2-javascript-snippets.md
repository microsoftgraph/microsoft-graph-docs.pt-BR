---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 90fed2b2e9a9869ac90d56c4e76aed48de47db6a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775364"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
   'template@odata.bind':'https://graph.microsoft.com/beta/teamsTemplates(\'educationClass\')',
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
    .version('beta')
    .post(team);

```