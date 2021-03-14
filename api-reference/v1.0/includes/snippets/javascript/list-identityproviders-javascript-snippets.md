---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d470a81b49fd0c37bb731ecd184ad18b48352a2e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806440"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identityProviders = await client.api('/identityProviders')
    .get();

```