---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61bed4df6a4efb4a179ecf23b512d708587c74bf1f9000c215b6cfc032cf79fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275732"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/range')
    .get();

```