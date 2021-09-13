---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f59eb48b35defcddd2aedb67f77f09f691e54068f1bd1767a1382f8980d39d86
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160141"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/tokenLifetimePolicies/{id}')
    .delete();

```