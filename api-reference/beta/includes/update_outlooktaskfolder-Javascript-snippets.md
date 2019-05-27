---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6559999e0a6c3f4f0bbb90efc77030e67993454f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: "Charity work"
};

let res = await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update({outlookTaskFolder : outlookTaskFolder});

```