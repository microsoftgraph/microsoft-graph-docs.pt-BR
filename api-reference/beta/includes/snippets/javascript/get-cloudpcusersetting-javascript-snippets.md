---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c922daee5883dbd24975b29e4dc47a69a1308449
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207297"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcUserSetting = await client.api('/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055')
    .version('beta')
    .get();

```