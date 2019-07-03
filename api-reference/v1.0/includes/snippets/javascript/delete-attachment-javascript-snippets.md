---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3eb47b24a9817ab36769678b240699889028a6a5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492634"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}/attachments/{id}')
    .delete();

```