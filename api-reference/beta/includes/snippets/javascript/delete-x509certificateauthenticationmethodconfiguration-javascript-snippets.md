---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4db7bba680a104550187efbf85607e1a8cb5809c
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/x509Certificate')
    .version('beta')
    .delete();

```