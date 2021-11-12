---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a0f5931389f599f127b06fd003f1214207cb5ef740ab61fea08a2027074af33
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  container: {
    url: 'https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874'
  },
  title: 'title-value'
};

await client.api('/planner/plans')
    .version('beta')
    .post(plannerPlan);

```