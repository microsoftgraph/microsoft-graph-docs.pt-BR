---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0d744d11440932827a139f4528055bad43d5ac90d01c24e344cb815d0333c47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let buckets = await client.api('/planner/buckets')
    .get();

```