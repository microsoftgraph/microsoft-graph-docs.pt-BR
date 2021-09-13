---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3272f86a24e7d6ccdc000e8e1fba3eda891719e180e08e163932cbc3ff1e654
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157896"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/servicePrincipals/{id}/getMemberObjects')
    .post(string);

```