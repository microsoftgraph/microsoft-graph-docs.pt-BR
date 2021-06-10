---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9990545c973eb22edd0f45f2182fc02dea9d0ca0
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869713"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect')
    .version('beta')
    .post();

```