---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9086dc22f63e02d31109fde29900693c8ed47d80
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35727400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365GroupsActivityCounts(period='D7')')
    .version('beta')
    .get();

```