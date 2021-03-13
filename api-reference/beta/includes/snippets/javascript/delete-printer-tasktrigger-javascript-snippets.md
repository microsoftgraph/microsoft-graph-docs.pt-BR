---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a2689f7754376a9d62ee94509b33cfc067ddadf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801185"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/1a5f91a7-9bd1-4d5f-bb86-f43554cac51c/taskTriggers/25be207e-1154-491f-aa68-a9f7007d4bec')
    .version('beta')
    .delete();

```