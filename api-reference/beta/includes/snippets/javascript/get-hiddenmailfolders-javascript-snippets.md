---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1871cce74dda0b351e9c44268434abeca6d36e1a
ms.sourcegitcommit: df0778a4dbd1e7a2fde1846bdfbfd9440fc91672
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/?includeHiddenFolders=true')
    .version('beta')
    .get();

```