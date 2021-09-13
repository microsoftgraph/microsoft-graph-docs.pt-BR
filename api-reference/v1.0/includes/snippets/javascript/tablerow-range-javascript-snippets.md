---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72392a99b27d5c4221220f9652048cc7fd1e86e19423dac0b0ff9b70d215df22
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookRange = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range')
    .get();

```