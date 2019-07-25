---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2902928dbc2e75b6319a76488d6252e53cb9437
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729136"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oAuth2Permissiongrants/{id}')
    .version('beta')
    .delete();

```