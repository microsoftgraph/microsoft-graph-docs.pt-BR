---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd6cb8f9ed204376ac11e381fa52593660e383a8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedApproval = await client.api('/privilegedApproval/{id}')
    .version('beta')
    .get();

```