---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fc3b65a3e2e92c0ee15c427194b6ef5863737dc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455067"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unprotect = {
  password: "password-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection/unprotect')
    .post(unprotect);

```