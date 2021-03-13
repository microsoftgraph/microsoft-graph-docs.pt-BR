---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 014f9834731ab4e6c7217ad3a9a66d2c5229d18c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}')
    .version('beta')
    .delete();

```