---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70b161ef9089e55aa7ad4eeda8dea30c1179295796d5a6711df011aa3410966b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57406718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/servicePrincipals/{id}/transitiveMemberOf')
    .get();

```