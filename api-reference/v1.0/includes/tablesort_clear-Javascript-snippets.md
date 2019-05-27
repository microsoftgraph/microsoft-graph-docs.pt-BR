---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: adebd9e3b62b79a0fc906bff06e0b9a01e956645
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear')
    .post();

```