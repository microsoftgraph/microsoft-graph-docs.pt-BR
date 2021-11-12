---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c34ae1a642e8bfc54f55537a8ec4dca321c592ec578f1bf5301496a47d97ff4f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rows = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows')
    .version('beta')
    .get();

```