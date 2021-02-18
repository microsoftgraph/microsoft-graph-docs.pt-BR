---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc6b28751739f17b27197689f81c44bd69c7aee0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274945"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/tokenIssuancePolicies/{id}/appliesTo')
    .get();

```