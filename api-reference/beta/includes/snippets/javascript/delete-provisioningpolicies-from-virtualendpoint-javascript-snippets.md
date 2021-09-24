---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56ade2f8697e7534d235445950415cef279181fb40c9721040ded4d55662d265
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies/{id}')
    .version('beta')
    .delete();

```