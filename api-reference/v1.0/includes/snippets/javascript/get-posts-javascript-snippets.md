---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd2ea7b6fc8bd396b33ca8f2a82ccb0db76c9150
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614568"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/threads/{id}/posts')
    .get();

```