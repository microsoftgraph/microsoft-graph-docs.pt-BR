---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46d6ac5bafa257a840563c40beb68d4e50c7bcbe
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35733707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityCounts(period='D7')')
    .get();

```