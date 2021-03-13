---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9945abb41ba30bd0c0350acbf7c088962a2df3a9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779803"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTaskFolder = {
  name: 'Charity work'
};

await client.api('/me/outlook/taskFolders/AAMkADIyAAAhrbPWAAA=')
    .version('beta')
    .update(outlookTaskFolder);

```