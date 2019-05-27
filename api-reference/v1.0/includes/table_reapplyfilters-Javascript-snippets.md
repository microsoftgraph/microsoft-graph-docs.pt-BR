---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 632ed65793b20a13ba5055337cdf5d59a5b2bd58
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters')
    .post();

```