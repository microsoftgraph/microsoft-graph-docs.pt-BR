---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7895147959df47bbd78d614574a148a9e2a1e1aaec04305dabc36b35ab9f5639
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375940"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTableRow = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .get();

```