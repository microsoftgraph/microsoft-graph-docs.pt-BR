---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a84995805aa1653f6cb1bccd1301aef8d1091fb1
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/email')
    .delete();

```