---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45c7feee81769947490d4b411bd5e7b226113ce0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groupSettings/{id}')
    .get();

```