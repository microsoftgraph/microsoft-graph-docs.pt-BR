---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cce6fad8723db0e0f781f026210404a86bb75c26
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690941"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/97a5a533-833d-494b-b543-c0afe026cb96/teamwork/installedApps')
    .filter('teamsApp/externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'')
    .expand('teamsAppDefinition')
    .get();

```