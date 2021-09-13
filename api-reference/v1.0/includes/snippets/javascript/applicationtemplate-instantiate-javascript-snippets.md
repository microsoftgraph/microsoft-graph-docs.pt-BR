---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5a6ca811ce2a0a6783166c785af67aa2df27e9027da0b6848f2f1e62efaf138
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const applicationServicePrincipal = {
  displayName: 'My custom name'
};

await client.api('/applicationTemplates/{id}/instantiate')
    .post(applicationServicePrincipal);

```