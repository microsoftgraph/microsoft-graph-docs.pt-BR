---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a780de21fde6c141938e45345ccda1f37fe3cbe3
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51922552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printerShare = {
  displayName: 'ShareName',
  allowAllUsers: true,
  'printer@odata.bind': 'https://graph.microsoft.com/beta/print/printers/{id}'
};

await client.api('/print/shares/{id}')
    .version('beta')
    .update(printerShare);

```