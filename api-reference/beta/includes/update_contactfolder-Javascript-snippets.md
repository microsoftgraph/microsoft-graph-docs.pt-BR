---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8695d8d32502b3fbbc92003300e3b34eb068b581
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475259"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  parentFolderId: "parentFolderId-value",
  displayName: "displayName-value"
};

let res = await client.api('/me/contactFolders/{id}')
    .version('beta')
    .update({contactFolder : contactFolder});

```