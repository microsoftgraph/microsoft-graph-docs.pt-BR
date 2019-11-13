---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c51f1d8b64ff82e9f5f4aa708869a9d506ba8f59
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302673"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/calls/{id}/audioRoutingGroups')
    .version('beta')
    .get();

```