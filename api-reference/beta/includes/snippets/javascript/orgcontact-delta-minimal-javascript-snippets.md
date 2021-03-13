---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 470fbb458fe550dfa37194dec977241e5155ab3e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .version('beta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mail')
    .get();

```