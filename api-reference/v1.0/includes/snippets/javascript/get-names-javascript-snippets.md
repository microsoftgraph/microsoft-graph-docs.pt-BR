---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1dcb60b90ee4ecc91171e147c1a232b65ffdd1e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names')
    .get();

```