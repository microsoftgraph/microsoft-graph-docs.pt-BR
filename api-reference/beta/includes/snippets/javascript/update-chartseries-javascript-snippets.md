---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 587cf9942965cfbe91b33baebec1fd2a9dce36da732b012af688da987464f451
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217027"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: 'name-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}')
    .version('beta')
    .update(workbookChartSeries);

```