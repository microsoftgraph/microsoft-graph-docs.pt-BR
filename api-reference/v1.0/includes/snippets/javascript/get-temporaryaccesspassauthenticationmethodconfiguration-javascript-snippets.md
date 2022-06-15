---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7c763b7c537c0a1c444c006c4612bc4019270e7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093200"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let authenticationMethodConfiguration = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/temporaryAccessPass')
    .get();

```