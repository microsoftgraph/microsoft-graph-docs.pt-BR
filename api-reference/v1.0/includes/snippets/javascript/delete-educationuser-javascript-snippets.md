---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c7902d1d0e753970b05ad8645786cb1018461be6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/users/{user-id}')
    .delete();

```