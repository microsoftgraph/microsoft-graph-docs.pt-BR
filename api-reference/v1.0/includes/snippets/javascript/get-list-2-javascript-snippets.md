---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 56fc7e8f000ee3a07955ae52971a0a724ba6b6eb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50956441"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let list = await client.api('/sites/{site-id}/lists/{list-title}')
    .get();

```