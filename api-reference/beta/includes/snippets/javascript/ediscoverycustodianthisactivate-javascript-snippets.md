---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e6f742c0e84190dced4109151fbb1056f0e14654
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095965"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{ediscoveryCustodianId}/activate')
    .version('beta')
    .post();

```