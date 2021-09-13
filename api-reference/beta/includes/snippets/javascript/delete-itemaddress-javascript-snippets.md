---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8f1667ed9c186bd618a93fc54a19a6555f911cadbb6be51d40e8463ae0a5322f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216585"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/addresses/{id}')
    .version('beta')
    .delete();

```