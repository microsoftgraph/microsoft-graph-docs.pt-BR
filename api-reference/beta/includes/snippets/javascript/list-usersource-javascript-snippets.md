---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 61b1943ac83a9b936f8dc104fbb421e042bda054
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let userSources = await client.api('/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources')
    .version('beta')
    .get();

```