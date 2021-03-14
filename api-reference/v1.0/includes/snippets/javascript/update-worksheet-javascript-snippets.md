---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4b6b5387d29ee3e5cfa437cc95eff744fe4986f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807702"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  position: 99,
  name: 'name-value',
  visibility: 'visibility-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}')
    .update(workbookWorksheet);

```