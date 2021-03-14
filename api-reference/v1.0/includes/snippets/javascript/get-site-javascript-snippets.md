---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 634977519a5641c31c867ae22ee50d7543d290e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803449"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let site = await client.api('/sites/{site-id}')
    .get();

```