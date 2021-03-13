---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d002b18df045770bae7f1f6bf03c05c7e92555c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781581"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscribedSkus = await client.api('/subscribedSkus')
    .version('beta')
    .get();

```