---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c19a59569110a6199af7bba04ae137ee952f4dc0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastCell')
    .get();

```