---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43915ed94ba5ba944e634d99c31a084fe76935b9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}')
    .get();

```