---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 683b69090b53aea48971a459829ce9b0cc0d9253
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartPoint = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/{point-id}')
    .get();

```