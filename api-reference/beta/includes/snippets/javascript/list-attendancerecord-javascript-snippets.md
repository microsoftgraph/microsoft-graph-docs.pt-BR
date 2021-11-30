---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d2b1521ee60df58d872b44e90c54fa8bbe6383f
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223571"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let attendanceRecords = await client.api('/me/onlineMeetings/{meetingId}/attendanceReports/{reportId}/attendanceRecords')
    .version('beta')
    .get();

```