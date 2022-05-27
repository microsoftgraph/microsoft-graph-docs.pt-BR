---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8943373acf60f04cda6f8834eecdf0066f11971beea99986f280c7ab7b044eb2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/tokenIssuancePolicies/{id}/$ref')
    .version('beta')
    .delete();

```