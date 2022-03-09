---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39e59b98507b863241ec7910cc9ef7e9406c2380
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393869"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let auditEvent = await client.api('/tenantRelationships/managedTenants/auditEvent')
    .version('beta')
    .get();

```