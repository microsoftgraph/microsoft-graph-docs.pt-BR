---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82f1cb1f10a9ffc8a514a8a001e3d203cf10ff2430d237feba147c530a3fb236
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274885"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/cloudPC/roleAssignments')
    .version('beta')
    .get();

```