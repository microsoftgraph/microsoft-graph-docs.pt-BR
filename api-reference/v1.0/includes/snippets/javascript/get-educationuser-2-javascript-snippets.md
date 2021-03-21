---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53d5c9c156c0bd8117c2a49b1627dd5548d60282
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationUser = await client.api('/education/users/{user-id}')
    .get();

```