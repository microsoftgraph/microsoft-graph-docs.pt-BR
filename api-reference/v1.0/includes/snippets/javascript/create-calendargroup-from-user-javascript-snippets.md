---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e13a9bf8900a38b00a3370c38966a99ddd11d111
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51506991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarGroup = {
  name: 'Personal events'
};

await client.api('/me/calendarGroups')
    .post(calendarGroup);

```