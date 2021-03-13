---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8317af6d5c44f346c9a9a62289976e9549d07284
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let taskTriggers = await client.api('/print/printers/{id}/taskTriggers')
    .version('beta')
    .get();

```