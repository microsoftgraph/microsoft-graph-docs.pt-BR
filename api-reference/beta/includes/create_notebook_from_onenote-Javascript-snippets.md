---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd13612a9e39d620b897c5d63d2ca748427d60b6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const notebook = {
  displayName: "Notebook name"
};

let res = await client.api('/me/onenote/notebooks')
    .version('beta')
    .post({notebook : notebook});

```