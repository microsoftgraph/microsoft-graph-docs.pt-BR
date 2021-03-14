---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 542c92f308436fd98b3cdbc598de61a63cc6996c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .get();

```