---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e2c6841d4db3fff8f9cb9921627a769b94c7240fca86456aa962d6c0f28180c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tokenLifetimePolicies = await client.api('/policies/tokenLifetimePolicies')
    .get();

```