---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45c7feee81769947490d4b411bd5e7b226113ce0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings/{id}')
    .get();

```