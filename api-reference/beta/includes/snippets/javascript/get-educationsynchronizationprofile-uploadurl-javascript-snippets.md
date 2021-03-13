---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f452d676c29c65f68872422d4d023487422bdcbc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782493"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let string = await client.api('/education/synchronizationProfiles/{id}/uploadUrl')
    .version('beta')
    .get();

```