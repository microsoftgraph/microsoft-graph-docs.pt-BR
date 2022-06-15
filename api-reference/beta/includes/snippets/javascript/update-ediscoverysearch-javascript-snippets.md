---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b493a55676a1385cacf5691cca6f8a7fc2a742c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092735"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const ediscoverySearch = {
    displayName: 'Teams search'
};

await client.api('/security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}')
    .version('beta')
    .update(ediscoverySearch);

```