---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02183908528d557dced9dcaf9f44a46af69efd20
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690334"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/appCatalogs/teamsApps')
    .filter('id eq 'b1c5353a-7aca-41b3-830f-27d5218fe0e5'')
    .get();

```