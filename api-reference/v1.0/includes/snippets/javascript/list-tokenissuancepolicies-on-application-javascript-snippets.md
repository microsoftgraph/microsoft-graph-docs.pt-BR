---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 194eea437454fdd67254a033a636d107710966e6d029250ab3495c8d9ea02511
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101097"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenIssuancePolicies = await client.api('/applications/{id}/tokenIssuancePolicies')
    .get();

```