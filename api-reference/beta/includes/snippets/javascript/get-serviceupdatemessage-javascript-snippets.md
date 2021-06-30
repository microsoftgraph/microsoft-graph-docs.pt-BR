---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8bd6a00419ebd6daa81b54e1341d4127ea9812f9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceUpdateMessage = await client.api('/admin/serviceAnnouncement/messages/MC172851')
    .version('beta')
    .get();

```