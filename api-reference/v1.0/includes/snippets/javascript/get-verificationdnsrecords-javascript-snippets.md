---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e601b6df65be2ea410f94015b417ff916e0db5df
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35466524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/domains/{domain-name}/verificationDnsRecords')
    .get();

```