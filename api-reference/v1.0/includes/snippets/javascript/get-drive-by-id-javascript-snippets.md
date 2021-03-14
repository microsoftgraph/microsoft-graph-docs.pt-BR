---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2be893122d587197154468e95965d3e346fa02a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779588"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let drive = await client.api('/drives/{drive-id}')
    .get();

```