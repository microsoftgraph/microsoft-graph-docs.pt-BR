---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e37f8fbd82bc98a1fb801bd2a32881c79560756c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471975"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates/{id}')
    .version('beta')
    .get();

```