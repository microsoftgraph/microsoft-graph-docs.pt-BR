---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2417cd8097557b1b9dd0e94b69b131e81eeea521
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let temporaryAccessPassMethods = await client.api('/users/071cc716-8147-4397-a5ba-b2105951cc0b/authentication/temporaryAccessPassMethods')
    .get();

```