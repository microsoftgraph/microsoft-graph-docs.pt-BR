---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 07c2ff3dda50b0f4d28ba92cba8f170e74a96a6d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460991"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/delta')
    .version('beta')
    .get();

```