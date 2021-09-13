---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a858a82dcefaffe44caaea2ee6fb39ef3f5249614bc081cc1f299e69ff0fabba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57375864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicies = await client.api('/applications/{id}/tokenLifetimePolicies')
    .get();

```