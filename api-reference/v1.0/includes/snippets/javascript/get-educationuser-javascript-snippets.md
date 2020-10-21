---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e232e352fc245a8739ecc9543f77a11e4ccb7835
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610461"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/{user-id}')
    .get();

```