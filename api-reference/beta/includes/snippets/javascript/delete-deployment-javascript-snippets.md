---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 163f1c97104aadf06d85359224f6249487f2f780
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52241374"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/admin/windows/updates/deployments/{deploymentId}')
    .version('beta')
    .delete();

```