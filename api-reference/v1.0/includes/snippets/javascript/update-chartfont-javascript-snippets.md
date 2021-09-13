---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c281921d717e70972adc31331e6cb1ef303525128b5a8ea77c58c74a68199849
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159516"
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

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font')
    .update(workbookChartFont);

```