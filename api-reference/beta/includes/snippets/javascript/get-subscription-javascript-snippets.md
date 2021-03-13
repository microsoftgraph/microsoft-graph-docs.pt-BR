---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 993d085025e326d2aca9e7e47344d8eff79f5a46
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let subscription = await client.api('/subscriptions/{id}')
    .version('beta')
    .get();

```