---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4832bfe5f63b90479bde58c8ad6caa0bbd7a2b2f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/oAuth2Permissiongrants/{id}')
    .version('beta')
    .get();

```