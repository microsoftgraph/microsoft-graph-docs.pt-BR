---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e601b6df65be2ea410f94015b417ff916e0db5df
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/verificationDnsRecords')
    .get();

```