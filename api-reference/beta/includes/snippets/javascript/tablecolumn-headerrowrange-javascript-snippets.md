---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79bd1c89dc495e5550807bd7db80a116adfed0d9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619163"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/{id|name}/HeaderRowRange')
    .version('beta')
    .post();

```