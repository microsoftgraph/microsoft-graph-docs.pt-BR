---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2631435d9207e1a0d42b8f2fe542a75f01ec581f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948670"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/appCatalogs/teamsApps?requiresReview=true')
    .post();

```