---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12ed15a8711f0407dacd99269928a9a29089dfdff5bef866f1107a7095d15cf8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273129"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/messages/{id}')
    .delete();

```