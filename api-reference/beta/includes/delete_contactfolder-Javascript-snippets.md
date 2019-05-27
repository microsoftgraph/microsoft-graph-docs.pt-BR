---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cbc07441eb6d9c75cae0124713be26fa029f85d7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438691"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/contactFolders/{id}')
    .version('beta')
    .delete();

```