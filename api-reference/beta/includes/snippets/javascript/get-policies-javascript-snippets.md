---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed9794eedfbd953c7ecb4c932febde2db8fa5642
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437549"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/conditionalAccess/policies')
    .version('beta')
    .filter('displayName eq \'SimplePolicy1\' or displayName eq \'SimplePolicy2\'')
    .get();

```