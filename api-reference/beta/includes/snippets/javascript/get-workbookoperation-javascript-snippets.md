---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e25af2c535a05c1827d96cc8d05a468ca179a93
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}')
    .version('beta')
    .get();

```