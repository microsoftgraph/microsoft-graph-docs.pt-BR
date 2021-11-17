---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8c91428b92a9b9205cba3185b465f7b5b371ef2372b7be8ff994a56177a2c34
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let legalHolds = await client.api('/compliance/ediscovery/cases/{caseId}/legalHolds')
    .version('beta')
    .get();

```