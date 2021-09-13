---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f903c8b3d202e42ab9833f33e9ed57c7f820e112
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59074469"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let device = await client.api('/devices/000005c3-b7a6-4c61-89fc-80bf5ccfc366')
    .get();

```