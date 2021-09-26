---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 382ee86ebb3ec16bd4d7ff7974768b9bc06cb0ed1dcd4c514763dc8ae69f0ef3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/onPremisesConnections/{id}/runHealthChecks')
    .version('beta')
    .post();

```