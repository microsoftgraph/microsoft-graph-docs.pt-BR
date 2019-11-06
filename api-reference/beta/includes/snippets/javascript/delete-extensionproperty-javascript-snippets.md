---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 77a301801cf45a7d3fcc6ce9da34962611125bb4
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37995559"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/extensionProperties/{id}')
    .version('beta')
    .delete();

```