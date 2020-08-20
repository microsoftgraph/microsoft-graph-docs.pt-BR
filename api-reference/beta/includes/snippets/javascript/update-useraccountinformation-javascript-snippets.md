---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8136f9b277eee8c10d412cae47ee1c68c3e549e6
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/20/2020
ms.locfileid: "46821337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const userAccountInformation = {
  countryCode: "NO"
};

let res = await client.api('/me/profile/account/{id}')
    .version('beta')
    .update(userAccountInformation);

```