---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c131e042e1e9abadd1315119414cc91181555f8c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782618"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}/send')
    .post();

```