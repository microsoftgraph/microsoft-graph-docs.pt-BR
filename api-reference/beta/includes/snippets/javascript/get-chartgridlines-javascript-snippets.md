---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: db5b2827752074c5915e85ff460d31a4eb288362c9283c89ba94e4ad542a7f55
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158917"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartGridlines = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/minorgridlines')
    .version('beta')
    .get();

```