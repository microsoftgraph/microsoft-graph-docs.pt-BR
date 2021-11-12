---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b55c8876b01f743e961b36ec0de4a4c94942924f56af7ae59da479cb00debb40
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158255"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationJob = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/')
    .version('beta')
    .get();

```