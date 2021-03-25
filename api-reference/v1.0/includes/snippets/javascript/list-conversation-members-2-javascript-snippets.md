---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eb07d678bad85dccaad3d56434ccc37c61390668
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51202346"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/chats/{id}/members')
    .get();

```