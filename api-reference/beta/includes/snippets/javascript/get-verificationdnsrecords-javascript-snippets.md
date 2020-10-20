---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc7443848049372502b239fae20d9fc0c5773eb2
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617151"
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