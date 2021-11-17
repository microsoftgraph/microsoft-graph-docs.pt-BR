---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1900559877fb00537bc50ba00e593db435f10a6450dd79f8db46d837e948d12
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272849"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/inferenceClassification/overrides/98f5bdef-576a-404d-a2ea-07a3cf34af4r')
    .version('beta')
    .delete();

```