---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f53e032db964cdd2c8c17369a17bfec17a3d11b363f9a6e26c9435552b9329b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160015"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerBucket = await client.api('/planner/buckets/{bucket-id}')
    .get();

```