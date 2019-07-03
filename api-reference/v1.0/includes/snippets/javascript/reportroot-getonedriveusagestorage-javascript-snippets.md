---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dfb983ccf82d4a8c171f7e960e90b950cd2a56e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOneDriveUsageStorage(period='D7')')
    .get();

```