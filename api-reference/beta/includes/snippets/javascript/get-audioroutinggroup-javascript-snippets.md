---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 345fe4022ba060be45276343da68d93d79b171c7
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/{id}/audioRoutingGroups/{id}')
    .version('beta')
    .get();

```