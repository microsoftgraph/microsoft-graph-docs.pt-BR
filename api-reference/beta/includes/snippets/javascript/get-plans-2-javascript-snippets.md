---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8113c1b352c7858f095a880c9b05bda3b3d1b0d22c0e2c268271ba2e5f9790bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326825"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/groups/ebf3b108-5234-4e22-b93d-656d7dae5874/planner/plans')
    .version('beta')
    .get();

```