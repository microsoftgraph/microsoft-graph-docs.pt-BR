---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe30208e1c8ad7e8e2fdbb69da0a53a3b9b468f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800751"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/clearFilters')
    .version('beta')
    .post();

```