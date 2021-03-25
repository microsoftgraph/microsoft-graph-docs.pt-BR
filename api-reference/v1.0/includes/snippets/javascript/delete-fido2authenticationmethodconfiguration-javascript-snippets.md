---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7658b078b05b268d2d0c78b4c81f627e073aca9f
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .delete();

```