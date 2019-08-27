---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27fd4dd9331fe3ecfba200e8b9a6de30015b236e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636208"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationTemplate = {
    id: "SCIM-Test1",
    applicationId: "{id}",
    factoryTag: "CustomSCIM"
};

let res = await client.api('/applications/{id}/synchronization/templates')
    .version('beta')
    .post(synchronizationTemplate);

```