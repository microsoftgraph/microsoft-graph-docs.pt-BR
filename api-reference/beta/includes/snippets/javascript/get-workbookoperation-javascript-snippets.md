---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9f7eb034b8512d3e08a2dfbcf9eee1691754700506a62595af4dba8883eabd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215132"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookOperation = await client.api('/me/drive/items/{drive-item-id}/workbook/operations/{operation-id}')
    .version('beta')
    .get();

```