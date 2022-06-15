---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a178c1f9ffa1267e1ac644f2892328b2ea1166ba
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094537"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods/05267842-25b2-4b21-8abd-8e4982796f7f')
    .delete();

```