---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3a136fdd9f52fea6cc55dfe1ed484682c7fe228
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: "embed"
};

let res = await client.api('/me/drive/items/{item-id}/createLink')
    .post(permission);

```