---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88d52bb444e42b4a9255a199bbbfa0c056452dc8
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718746"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')')
    .version('beta')
    .get();

```