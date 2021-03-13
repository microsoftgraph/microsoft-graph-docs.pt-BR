---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e87239ee228dfd2bc9e81d785ec7e7e251a59784
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/applications/{id}/extensionProperties/{id}')
    .version('beta')
    .delete();

```