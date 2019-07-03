---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc7443848049372502b239fae20d9fc0c5773eb2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/contoso.com/verificationDnsRecords')
    .version('beta')
    .get();

```