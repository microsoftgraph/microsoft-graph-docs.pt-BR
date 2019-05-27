---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ceef1c821a09e46b32dda78efe03e6cafb48865f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/range')
    .post();

```