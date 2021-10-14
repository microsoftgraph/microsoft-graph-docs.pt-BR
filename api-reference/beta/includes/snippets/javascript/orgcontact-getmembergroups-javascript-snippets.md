---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39c53130ca160cdba4d4f133701bd861eabb41c6d871914639839791396a296b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159943"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/contacts/{id}/getMemberGroups')
    .version('beta')
    .post(string);

```