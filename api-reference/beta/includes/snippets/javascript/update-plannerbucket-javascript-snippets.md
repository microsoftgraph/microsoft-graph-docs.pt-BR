---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f974dac87b433032b63f71a8f69892895785a3a4dc8eb270d9cf6bdff53e01b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159205"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: 'Development'
};

await client.api('/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR')
    .version('beta')
    .update(plannerBucket);

```