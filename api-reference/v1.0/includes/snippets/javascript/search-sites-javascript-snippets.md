---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b86f82b6b1ee821148334259e5378d7751afdbd1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604701"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites?search=%7Bquery%7D')
    .get();

```