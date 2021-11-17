---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7964ad2797274da8f9bb9653a26d874d12dcdbca427269b8c238e88afcb96e61
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214576"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocations = await client.api('/identity/conditionalAccess/namedLocations')
    .version('beta')
    .filter('isof(\'microsoft.graph.ipNamedLocation\')')
    .get();

```