---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 95b784453a93166627ad260efe664a30605e7ca392ce5cca2dcff386037a356a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  index: 8
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/itemAt')
    .post(workbookChart);

```