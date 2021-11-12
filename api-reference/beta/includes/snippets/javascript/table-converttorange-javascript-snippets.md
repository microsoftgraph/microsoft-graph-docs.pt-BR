---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2e2d3740842d09ca82c1056d27273445c520b2af56d84b0a511ce143421c506
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159613"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/convertToRange')
    .version('beta')
    .post();

```