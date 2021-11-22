---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7320a46dcf7ba1dc9b8ea8eb9f234bd7393d4bd053a3249fb0b94deaf1f586d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}')
    .version('beta')
    .delete();

```