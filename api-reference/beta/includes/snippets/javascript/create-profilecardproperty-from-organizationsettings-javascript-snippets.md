---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5aa0a248332463e5cb91703bffcf1dcb5f601af445e754b85ca715be1804f92b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const profileCardProperty = {
  directoryPropertyName: 'CustomAttribute1',
  annotations: [
    {
      displayName: 'Cost Center',
      localizations: [
        {
          languageTag: 'ru-RU',
          displayName: 'центр затрат'
        }
      ]
    }
  ]
};

await client.api('/organization/{organizationId}/settings/profileCardProperties')
    .version('beta')
    .post(profileCardProperty);

```