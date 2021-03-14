---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5e8f2a7d040b365751e5502e84f119d3d6b425d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/range')
    .get();

```