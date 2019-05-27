---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1f58c2ab4589b30baa76c858503dea8a843d354
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/security/securityActions/{id}')
    .version('beta')
    .get();

```