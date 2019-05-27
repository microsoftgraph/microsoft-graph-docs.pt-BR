---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e09613a2363b5af1a2c13b71254121b04b7c2565
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
    clientSecret: "1111111111111"
};

let res = await client.api('/identityProviders/Amazon-OAuth')
    .version('beta')
    .update({identityProvider : identityProvider});

```