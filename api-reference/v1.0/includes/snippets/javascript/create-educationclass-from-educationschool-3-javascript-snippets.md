---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f5f599e3a562de7a08f92ca8e2d0a0c6d246a83c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956591"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/schools/{school-id}/classes/{class-id}')
    .delete();

```