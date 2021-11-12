---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8467bffe3b46267cfe5a2553e56f3bc0c3158fe52e9472372b35cf247446a63f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899636"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  id: '99',
  name: 'name-value',
  index: 99,
  values: 'values-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .version('beta')
    .post(workbookTableColumn);

```