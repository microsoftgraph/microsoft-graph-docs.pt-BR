---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8936d8963902f910742a2b97254381ce3fc6ab2674487613a5be002db3fbb42f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/headerRowRange')
    .get();

```