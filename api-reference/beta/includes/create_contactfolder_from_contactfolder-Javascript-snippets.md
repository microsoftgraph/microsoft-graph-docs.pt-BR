---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c82f8b7c73f8d346113249be4c79a56b8ac88777
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457021"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contactFolder = {
  displayName: "displayName-value"
};

let res = await client.api('/me/contactFolders/{id}/childFolders')
    .version('beta')
    .post({contactFolder : contactFolder});

```