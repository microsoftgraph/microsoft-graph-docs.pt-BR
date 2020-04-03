---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62f90c50ec9591332e9f2e7ce1f1b6406fc369d2
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123184"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/drives/{drive-id}/items/{item-id}/getActivitiesByInterval(startDateTime='2017-01-01',endDateTime='2017-01-3',interval='day')')
    .version('beta')
    .get();

```