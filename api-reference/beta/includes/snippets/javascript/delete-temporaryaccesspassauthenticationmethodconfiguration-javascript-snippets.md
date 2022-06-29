---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7dd3a58fe35410dcd3fa1d94f1d0512b9a2476d
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass`')
    .version('beta')
    .delete();

```