---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71ce9edf12294423d7754a76b77756d6bfde32c4233f966bfc64db3418f7758b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: 'A6673H Ejkl!'
};

await client.api('/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat')
    .version('beta')
    .update(plannerBucketTaskBoardTaskFormat);

```