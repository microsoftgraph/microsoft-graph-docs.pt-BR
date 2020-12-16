---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3131ac454640543c6d88ff55cf07aeb04e607064
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/acda442c-78d2-491b-8204-4ef5019c0193/installedApps')
    .filter('teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'')
    .expand('teamsAppDefinition')
    .get();

```