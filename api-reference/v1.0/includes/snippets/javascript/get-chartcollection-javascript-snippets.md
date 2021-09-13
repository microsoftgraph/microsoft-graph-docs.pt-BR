---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82bcb1f8bafcb93bc3e09f443e943cd9f002a18f8666508d5384f984680b1551
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let charts = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .get();

```