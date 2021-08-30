---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2746ca3261571b4e2ef86d820854311bcebbaea4b704af0b1d1133d8d2861908
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899047"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let servicePrincipal = await client.api('/servicePrincipals/{id}')
    .version('beta')
    .get();

```