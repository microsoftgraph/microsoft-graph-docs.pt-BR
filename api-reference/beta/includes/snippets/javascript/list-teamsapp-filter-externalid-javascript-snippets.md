---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7393d3ddb069aae419280e92a82531c19235d5c9
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .version('beta')
    .filter('externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'')
    .get();

```