---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd7ce10851ec023954c991800dad675b354ec01a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  clientSecret: '1111111111111'
};

await client.api('/identityProviders/Amazon-OAuth')
    .version('beta')
    .update(identityProvider);

```