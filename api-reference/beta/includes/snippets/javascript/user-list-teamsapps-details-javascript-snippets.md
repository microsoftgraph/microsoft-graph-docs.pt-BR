---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d15578e412209724667b190b70a76b4939ff1786
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691290"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/teamwork/installedApps')
    .version('beta')
    .expand('teamsAppDefinition')
    .get();

```