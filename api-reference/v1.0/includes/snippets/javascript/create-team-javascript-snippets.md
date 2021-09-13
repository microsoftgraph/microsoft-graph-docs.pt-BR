---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f705d80f75794cb44a01d881fd96fbd624c1cfdcec740df5627c0cbbeff4b8d3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217045"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  memberSettings: {
    allowCreatePrivateChannels: true,
    allowCreateUpdateChannels: true
  },
  messagingSettings: {
    allowUserEditMessages: true,
    allowUserDeleteMessages: true
  },
  funSettings: {
    allowGiphy: true,
    giphyContentRating: 'strict'
  }
};

await client.api('/groups/{id}/team')
    .put(team);

```