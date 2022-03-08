---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5bc5b78fb2edbb8d5b5ad77f20820e808862878
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let event = await client.api('/me/events/AAMkADAGAADDdm4NAAA=/')
    .version('beta')
    .expand('exceptionOccurrences,cancelledOccurrences')
    .select('subject,start,end,occurrenceId,exceptionOccurrences,cancelledOccurrences')
    .get();

```