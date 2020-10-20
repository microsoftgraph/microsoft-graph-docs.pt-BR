---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc3c38d89208857d5c5885bed7332f0ffb97125f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels')
    .version('beta')
    .get();

```