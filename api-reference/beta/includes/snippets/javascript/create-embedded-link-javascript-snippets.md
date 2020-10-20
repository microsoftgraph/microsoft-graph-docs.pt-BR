---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3543fc8f60316c94e9dba4bc25541d7d3e6e87de
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610717"
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
    .version('beta')
    .post(permission);

```