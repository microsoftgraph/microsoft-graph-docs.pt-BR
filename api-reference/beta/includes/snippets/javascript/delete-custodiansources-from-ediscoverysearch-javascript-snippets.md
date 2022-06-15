---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72584225513d1f9a7eec3834dee9996e1e9f4f7b
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/custodianSources/{id}/$ref')
    .version('beta')
    .delete();

```