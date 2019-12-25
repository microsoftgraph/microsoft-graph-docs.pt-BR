---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b786b31d3ee1420bf138baa9cf9eb8934d2f2015
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867118"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/informationProtection/threatAssessmentRequests/ab2ad9b3-2213-4091-ae0c-08d76ddbcacf')
    .version('beta')
    .get();

```