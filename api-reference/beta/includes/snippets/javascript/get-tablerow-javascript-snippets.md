---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb13da6115bad2716886a1cbe5590961c8c9a6ff9db9b7f496d0a43bd7680346
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273516"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableRow = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .version('beta')
    .get();

```