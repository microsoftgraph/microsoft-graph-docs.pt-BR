---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b9fa986cfb6098868a94de980bd7d1b84316dde8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470498"
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
    .post({contactFolder : contactFolder});

```