---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24744fa7454bd8402e16c958f58dded8f9d9b7c8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809557"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schema = await client.api('/external/connections/contosohr/schema')
    .version('beta')
    .get();

```