---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40c95ab66f5a63324f801be84cf818fb33dda138
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScore = await client.api('/security/secureScores/{id}')
    .get();

```