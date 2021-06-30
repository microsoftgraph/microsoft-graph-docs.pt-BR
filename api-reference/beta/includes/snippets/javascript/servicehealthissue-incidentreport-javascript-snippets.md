---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26846e2cca553bf6a0e50f79a3b68fdedff4e530
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let stream = await client.api('/admin/serviceAnnouncement/issues/MO248163/incidentReport')
    .version('beta')
    .get();

```