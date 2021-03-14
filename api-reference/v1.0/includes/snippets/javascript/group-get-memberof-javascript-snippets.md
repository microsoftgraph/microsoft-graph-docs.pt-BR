---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 482053b58815cab8ee2ab391794f27500c02099b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791230"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/groups/{id}/memberOf')
    .get();

```