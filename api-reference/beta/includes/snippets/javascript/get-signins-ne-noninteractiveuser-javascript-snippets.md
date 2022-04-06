---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6ac37c1abd516c037206aaef144a2fafc2e36cb7
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signins')
    .version('beta')
    .filter('(signInEventTypes/any(t: t ne \'interactiveUser\'))')
    .orderby('createdDateTime DESC')
    .top(10)
    .get();

```