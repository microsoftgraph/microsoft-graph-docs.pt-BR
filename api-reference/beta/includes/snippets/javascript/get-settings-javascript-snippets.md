---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e64864d736a7cee89898b819ea78cb9466cc6b86
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let settings = await client.api('/compliance/ediscovery/cases/5b840b94-f821-4c4a-8cad-3a90062bf51a/settings')
    .version('beta')
    .get();

```