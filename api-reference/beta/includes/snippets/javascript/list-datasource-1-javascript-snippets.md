---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2fe8be0fabb6d31edc5b7685d4ca452d81c1edd
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952137"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let additionalSources = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/additionalSources')
    .version('beta')
    .get();

```