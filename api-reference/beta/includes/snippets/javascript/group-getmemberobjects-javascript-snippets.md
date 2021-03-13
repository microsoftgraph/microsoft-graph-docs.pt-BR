---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c29fd053460e3b77b1ef0116a707dee977f53149
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799083"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/groups/{id}/getMemberObjects')
    .version('beta')
    .post(string);

```