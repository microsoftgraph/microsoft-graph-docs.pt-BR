---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c19a59569110a6199af7bba04ae137ee952f4dc0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/lastCell')
    .get();

```