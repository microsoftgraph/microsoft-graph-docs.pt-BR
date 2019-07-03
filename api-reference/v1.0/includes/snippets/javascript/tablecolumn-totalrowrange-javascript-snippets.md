---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 990af52386f1444fb50e2d2a88027115d185a92e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492341"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/totalRowRange')
    .post();

```