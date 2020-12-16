---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6f3c04656f7202b842414a4d66bd0d84eee2533
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49692634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{id}/installedApps/{id}')
    .expand('teamsAppDefinition')
    .get();

```