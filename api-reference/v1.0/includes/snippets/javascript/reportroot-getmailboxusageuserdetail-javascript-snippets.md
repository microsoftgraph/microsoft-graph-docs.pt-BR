---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 269aac21c2b9eca0f425e49ec780d0b7ca88a44d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507578"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getMailboxUsageDetail(period='D7')')
    .get();

```