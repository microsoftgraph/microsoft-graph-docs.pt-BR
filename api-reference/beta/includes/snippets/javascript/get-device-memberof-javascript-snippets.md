---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 151f5502ebaccdcd4433723e78fd79a5eecf0551104e486e9b0f769f0f34309a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/devices/{id}/memberOf')
    .version('beta')
    .get();

```