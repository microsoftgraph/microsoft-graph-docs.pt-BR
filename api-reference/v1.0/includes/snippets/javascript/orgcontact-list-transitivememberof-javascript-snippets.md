---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee225230b0ba5552841bc7f93bedff815c93bc7c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773456"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/contacts/{id}/transitiveMemberOf')
    .get();

```