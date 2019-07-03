---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 454f962d528d78da0bd886fcbda879896d332993
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492552"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/createForward')
    .post();

```