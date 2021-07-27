---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4ae377e12eab02766a9cee8028278297b72f261
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580534"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let availableProviderTypes = await client.api('/identity/identityProviders/availableProviderTypes')
    .get();

```