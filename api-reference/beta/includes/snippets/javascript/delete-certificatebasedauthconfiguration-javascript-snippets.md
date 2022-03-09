---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2ef57f4334082b60371dc9e4dd08a0c4fa5158ea4af0e66a0989b9058b6792ac
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/organization/{id}/certificateBasedAuthConfiguration/{id}')
    .version('beta')
    .delete();

```