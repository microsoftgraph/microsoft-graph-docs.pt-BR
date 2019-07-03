---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce99740ccabce8c45740c1a9f663e384e0bca310
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityUserDetail(period='D7')')
    .version('beta')
    .get();

```