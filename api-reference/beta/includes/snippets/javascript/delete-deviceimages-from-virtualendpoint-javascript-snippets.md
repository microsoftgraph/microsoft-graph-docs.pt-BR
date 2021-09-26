---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5dbeb4dff6e35bb5886b9bd2c5757cb72a081d26b568038d254b27e2b2d9b435
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897952"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/deviceManagement/virtualEndpoint/deviceImages/{id}')
    .version('beta')
    .delete();

```