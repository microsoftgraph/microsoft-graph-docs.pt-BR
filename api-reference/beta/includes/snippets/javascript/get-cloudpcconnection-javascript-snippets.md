---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35269e9735db7767f50e39ffb92d006754c1a6de
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcConnection = await client.api('/tenantRelationships/managedTenants/cloudPcConnections/86789ee0-e31d-4bee-98e6-6f310bd327bb')
    .version('beta')
    .get();

```