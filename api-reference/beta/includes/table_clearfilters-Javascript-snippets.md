---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e362800b9ff4d854d7a4e726097ba180ede1654b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465892"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters')
    .version('beta')
    .post();

```