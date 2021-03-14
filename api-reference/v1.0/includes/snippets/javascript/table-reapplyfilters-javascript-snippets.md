---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1713342e2c859a372a7fd6366fe722fc9f5ed749
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/reapplyFilters')
    .post();

```