---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97beab7b3e4d59d463a72317fa1c46c53ce64f4c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSharePointSiteUsageSiteCounts(period='D7')')
    .get();

```