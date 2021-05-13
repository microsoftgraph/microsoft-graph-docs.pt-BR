---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f776d5457ae8a24fe05b5ec67d5b4e3543dd90b9
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52476760"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const group = {
   description: 'description-value',
   displayName: 'displayName-value'
};

await client.api('/groups/{id}')
    .version('beta')
    .update(group);

```