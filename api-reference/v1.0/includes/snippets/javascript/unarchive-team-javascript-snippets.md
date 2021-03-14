---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd02f44d13b59eb024a238634ecaeb5369231e84
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802409"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{id}/unarchive')
    .post();

```