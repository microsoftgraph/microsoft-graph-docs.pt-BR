---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b7c338376fac7b3c9631ef465746c3eab684209e994853d1a2c453e6c01df2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSynchronizationProfileStatus = await client.api('/education/synchronizationProfiles/{id}/profileStatus')
    .version('beta')
    .get();

```