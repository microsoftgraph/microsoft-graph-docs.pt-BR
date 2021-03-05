---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf3c91951f769a80609a023a3be70cd548ef7ad2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470491"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let synchronizationProfiles = await client.api('/education/synchronizationProfiles')
    .version('beta')
    .get();

```