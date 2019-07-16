---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9270b7997c17b1f1706bb36119eb28620f6a88ad
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta')
    .header('Prefer','odata.maxpagesize=2')
    .skiptoken('R0usmcCM996atia_s')
    .get();

```