---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bdafce7112cdb7bdccd5feeeff60822d0c7ec5db
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/settings/resetToDefault')
    .version('beta')
    .post();

```