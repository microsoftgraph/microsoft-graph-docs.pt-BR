---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03b975ebc1150dd596cc374be6c548c6ddc0df14
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470379"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let educationSynchronizationProfile = await client.api('/education/synchronizationProfiles/{id}')
    .version('beta')
    .get();

```