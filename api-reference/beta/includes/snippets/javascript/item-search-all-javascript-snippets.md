---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e38a8af127b6c9614f9e11afb4ee7c8a8e4ebae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let search = await client.api('/me/drive/search(q='Contoso Project')')
    .version('beta')
    .get();

```