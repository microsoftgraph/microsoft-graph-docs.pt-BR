---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8744220d6f87e42ccfbfc440c30c7b383d5b99b1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771355"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printOperation = await client.api('/print/operations/{printOperationId}')
    .get();

```