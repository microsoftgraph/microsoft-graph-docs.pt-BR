---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6f193d34693653d25ae8a561e526f9aa1cd44ee85e5a63f634da0ba8dbd9f92
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899203"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/me/getMemberGroups')
    .post(string);

```