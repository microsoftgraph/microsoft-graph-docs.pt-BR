---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6629c55d86413ac2c81a021caec2a878affb4c60
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784165"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartFont = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font')
    .get();

```