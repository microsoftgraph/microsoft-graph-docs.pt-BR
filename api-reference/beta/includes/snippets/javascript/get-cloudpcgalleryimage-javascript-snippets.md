---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2309474883620616d04efe29bd49b69867fd7273
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2021
ms.locfileid: "60891102"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcGalleryImage = await client.api('/deviceManagement/virtualEndpoint/galleryImages/{id}')
    .version('beta')
    .get();

```