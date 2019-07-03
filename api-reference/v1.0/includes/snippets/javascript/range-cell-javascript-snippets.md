---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c20ac73b38f3a8d406927f0494391d8d9bba6f66
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508437"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/cell(row=5,column=6)')
    .get();

```