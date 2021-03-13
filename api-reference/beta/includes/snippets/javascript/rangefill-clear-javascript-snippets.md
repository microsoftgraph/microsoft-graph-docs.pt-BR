---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 888b498e9dbe991d4bd52d6edc15da1d9cd97c04
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809743"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill/clear')
    .version('beta')
    .post();

```