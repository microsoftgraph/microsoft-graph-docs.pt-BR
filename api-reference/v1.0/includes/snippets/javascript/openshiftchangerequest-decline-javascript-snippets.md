---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8b41ae3d261174c965028a68a43960a94faa1440a3de9ece9b9c5edf0da07bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: 'message-value'
};

await client.api('/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline')
    .post(decline);

```