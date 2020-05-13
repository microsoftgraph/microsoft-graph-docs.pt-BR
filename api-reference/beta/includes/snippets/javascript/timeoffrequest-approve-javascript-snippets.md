---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0de9bcf162b745a43bfaa1bb2f90b99d4331ee14
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217126"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: "message-value"
};

let res = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve')
    .version('beta')
    .post(approve);

```