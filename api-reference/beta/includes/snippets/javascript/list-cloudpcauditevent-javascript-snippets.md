---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 390e6bc3500a3ab359721652ddea6981e808808d
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316566"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let auditEvents = await client.api('/deviceManagement/virtualEndpoint/auditEvents')
    .version('beta')
    .get();

```