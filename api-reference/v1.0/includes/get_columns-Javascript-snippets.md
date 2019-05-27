---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b98883f776fec951fcf964500da56397b26203e3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34467668"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .skip(5)
    .top(5)
    .get();

```