---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c24e32f639ea0545eeec832399369afbcba2fcebe40c390b7f7533ea5d5e0563
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let charts = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .version('beta')
    .get();

```