---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38e68692f41bf0ce0686bb9d426fed2d7af582e5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781899"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
 isMembershipLimitedToOwners: true,
  memberSettings: {
    allowCreateUpdateChannels: true
  },
  messagingSettings: {
    allowUserEditMessages: true,
    allowUserDeleteMessages: true
  },
  funSettings: {
    allowGiphy: true,
    giphyContentRating: 'strict'
  },
  discoverySettings: {
    showInTeamsSearchAndSuggestions: true
  }
};

await client.api('/teams/{id}')
    .version('beta')
    .update(team);

```