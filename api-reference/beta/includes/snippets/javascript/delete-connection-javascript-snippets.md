---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 346ea010a78341585c0539ea238408bc4b811f72
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800176"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/connections/contosohr')
    .version('beta')
    .delete();

```