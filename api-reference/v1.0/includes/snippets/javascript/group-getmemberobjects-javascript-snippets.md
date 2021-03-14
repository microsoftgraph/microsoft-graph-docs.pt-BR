---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1e4136fa4da71e39c7f55e119c5d591ac31462c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802589"
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
    .post(string);

```