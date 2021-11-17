---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d5662146428834fd4ab82dd04c32068f6e0eb30aa5d505916753266a95a27173
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273196"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/tokenLifetimePolicies/{id}')
    .version('beta')
    .delete();

```