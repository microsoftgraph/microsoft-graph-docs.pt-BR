---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2786b01823072cc32116d3af927717ae46259a559780ddf690c1483f762319c3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216109"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartSeries = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}')
    .get();

```