---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 387002883b244f13655b0541792bb9e4296574e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796877"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/users/{id}/memberOf')
    .get();

```