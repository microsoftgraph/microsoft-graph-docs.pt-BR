---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aed43f394599b5694ac9b806ce2fdf21978223c10070271c0b5f4b6e09fc1294
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookTable = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}')
    .get();

```