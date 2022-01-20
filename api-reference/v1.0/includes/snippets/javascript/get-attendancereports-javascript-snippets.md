---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad3deda2374c3ffe6180e35d36f292ffa7a5cdc0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attendanceReports = await client.api('/me/onlineMeetings/MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZ/attendanceReports')
    .get();

```