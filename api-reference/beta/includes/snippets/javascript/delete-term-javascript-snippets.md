---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 535f90e577cf57e94e5edfd2d04a5a3ca0d17617cd2f5cf6116657f564f9228d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273204"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/termStore/sets/{setId}/terms/{termId}')
    .version('beta')
    .delete();

```