---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3507dbe788f023c87e6c86fe56cbcbd959425039fb5e445716b81129c2c7882
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100236"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

await client.api('/contacts/{id}/getMemberGroups')
    .post(string);

```