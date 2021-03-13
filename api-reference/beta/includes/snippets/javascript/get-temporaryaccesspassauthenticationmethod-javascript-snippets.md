---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecf59aee355ac5f1bd395c88a197be79fe55c5cd
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810113"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassAuthenticationMethod = await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods/30fd0dfc-0dfc-30fd-fc0d-fd30fc0dfd30')
    .version('beta')
    .get();

```