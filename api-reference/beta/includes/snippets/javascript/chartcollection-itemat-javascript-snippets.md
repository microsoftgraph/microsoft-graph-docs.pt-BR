---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb95e74beb0e027a5d6fbf01db316025a70b46941b27c609c4609fb9ce9d631b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157117"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  index: 8
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/ItemAt')
    .version('beta')
    .post(workbookChart);

```