---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9641bc9b1a7cba3ca7d05eb2194a825c9f3250a70e2d7ef981665c51a776dfaf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let namedLocation = await client.api('/identity/conditionalAccess/namedLocations/0854951d-5fc0-4eb1-b392-9b2c9d7949c2')
    .version('beta')
    .get();

```