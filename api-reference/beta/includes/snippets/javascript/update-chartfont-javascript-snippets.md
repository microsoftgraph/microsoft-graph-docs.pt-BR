---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 679bc017e1be1d53daa853a390cfcbae53b2ee9d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803192"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartFont = {
  bold: true,
  color: 'color-value',
  italic: true,
  name: 'name-value',
  size: 99,
  underline: 'underline-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font')
    .version('beta')
    .update(workbookChartFont);

```