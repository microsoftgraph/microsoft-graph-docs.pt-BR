---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e0a1cd5d8ebf51ae300ffb2134e7536ba7b476b8879179703024d42703d814c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156904"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterOperators = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/filterOperators')
    .version('beta')
    .get();

```