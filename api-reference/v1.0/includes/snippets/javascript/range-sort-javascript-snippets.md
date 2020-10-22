---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2a76e6b52174fd503c3d0917f4b1915095bf176
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620701"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/sort')
    .get();

```