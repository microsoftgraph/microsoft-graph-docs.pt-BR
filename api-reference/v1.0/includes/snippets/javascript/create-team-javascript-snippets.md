---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6aa594adc83f45cfd10f963e7c97ac2a1ccd14bd
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44866553"
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
    giphyContentRating: "strict"
  }
};

let res = await client.api('/groups/{id}/team')
    .put(team);

```