---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74dd96da036bfd2456d439d9758e20a2832870a47ef8fbe10f4ad309837ea9bf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102485"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerBucket = await client.api('/planner/buckets/hsOf2dhOJkqyYYZEtdzDe2QAIUCR')
    .version('beta')
    .get();

```