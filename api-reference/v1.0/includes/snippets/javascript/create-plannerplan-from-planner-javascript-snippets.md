---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a095e533f3639f5efe83b4123dc0a2963b11e0d67395ad94c61b3cd3772684c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  owner: 'ebf3b108-5234-4e22-b93d-656d7dae5874',
  title: 'title-value'
};

await client.api('/planner/plans')
    .post(plannerPlan);

```