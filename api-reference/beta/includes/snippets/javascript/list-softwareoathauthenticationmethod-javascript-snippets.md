---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f3df6fd6e888abc4e8d9532d72e8dd928235a34
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "60995200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let softwareOathMethods = await client.api('/me/authentication/softwareOathMethods')
    .version('beta')
    .get();

```