---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06c32a779709ce8e90e8980afd2898f4fc40e08a
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/6903fa93-605b-43ef-920e-77c4729f8258/installedApps')
    .version('beta')
    .get();

```