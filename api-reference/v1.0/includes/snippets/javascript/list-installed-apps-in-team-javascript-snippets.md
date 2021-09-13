---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97085a93d01330e617cf5f70fbb3605fc8cc507e4a8770957a398d561e1dd252
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let installedApps = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps')
    .get();

```