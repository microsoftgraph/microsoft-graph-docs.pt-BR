---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d4c2cda573ab4398fb5928f417a104f882200de52005294ac592ffdc7239c57
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeCards = await client.api('/teams/fd15cad8-80f6-484f-9666-3caf695fbf32/schedule/timeCards')
    .version('beta')
    .filter('state eq \'clockedOut\'')
    .top(2)
    .get();

```