---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5af47a15f49a64234aa77197e4b5a06cb28f7fd1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/{class-id}/teachers/{teacher-id}')
    .delete();

```