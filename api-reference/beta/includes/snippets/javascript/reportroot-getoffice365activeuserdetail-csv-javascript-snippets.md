---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 744d52ee0740329f903d8feca9b4288ac8119135
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35719295"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActiveUserDetail(period='D7')')
    .version('beta')
    .get();

```