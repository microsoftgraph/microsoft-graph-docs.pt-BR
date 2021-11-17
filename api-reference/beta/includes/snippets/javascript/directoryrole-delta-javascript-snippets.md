---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8023328d35913b629a131b50941b8ffe93c52ce9ff30f515628db9d41d0a453d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216905"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/directoryRoles/delta')
    .version('beta')
    .get();

```