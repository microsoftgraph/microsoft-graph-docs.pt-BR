---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef9fc33a4580ff1b581315577bc241b7aed09976
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458834"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupLifecyclePolicies/{id}')
    .delete();

```