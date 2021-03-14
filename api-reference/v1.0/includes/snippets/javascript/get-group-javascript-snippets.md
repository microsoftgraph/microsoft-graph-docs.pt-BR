---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6997ec982f6d0bd9a6ddf5404f4a32c474f2e203
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let group = await client.api('/groups/b320ee12-b1cd-4cca-b648-a437be61c5cd')
    .get();

```