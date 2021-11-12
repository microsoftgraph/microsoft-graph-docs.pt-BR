---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dba8c0f5e1cdd67f169243d9617748cd29bf3f07f412f161d2bc7a30a6241f3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160245"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/planner/plans')
    .version('beta')
    .get();

```