---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a20171f0ab6a8156e9647c59afc02cd3f56766e4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userAccountInformation = {
  countryCode: 'NO'
};

await client.api('/me/profile/account/{id}')
    .version('beta')
    .update(userAccountInformation);

```