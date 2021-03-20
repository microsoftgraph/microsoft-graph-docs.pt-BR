---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01551a0a1eab36ab1f2631b9fd1ebd739ecc3b93
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plans = await client.api('/planner/plans')
    .get();

```