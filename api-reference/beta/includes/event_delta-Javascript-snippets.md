---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 918d73c1863df00e4b4f473a154ae77d6b17b232
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarview/delta?startdatetime=%7Bstart_datetime%7D&enddatetime=%7Bend_datetime%7D')
    .version('beta')
    .get();

```