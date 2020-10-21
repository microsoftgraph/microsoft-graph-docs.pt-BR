---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba7460c48936867212a328eadb548a6bd7c0c96d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604913"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/resources/{id}/content')
    .get();

```