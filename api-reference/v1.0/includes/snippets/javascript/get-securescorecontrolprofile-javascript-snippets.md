---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84844d4bb6cb8cf54a0d9dc42be3bc499c2faa58
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795228"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let secureScoreControlProfile = await client.api('/security/secureScoreControlProfiles/{id}')
    .get();

```