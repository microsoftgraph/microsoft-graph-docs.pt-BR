---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4df5f224c1af96c718704ca36e62d18e5b14794f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783340"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .delete();

```