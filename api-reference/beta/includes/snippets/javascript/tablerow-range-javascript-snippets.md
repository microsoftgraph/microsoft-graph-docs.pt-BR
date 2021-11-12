---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2258949a4453d885a11af48ad755da5748c110302119b511ca055ccf2fd2529
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/Range')
    .version('beta')
    .get();

```