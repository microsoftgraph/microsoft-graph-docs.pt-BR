---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a01c55c7670b07d69db70c83f4807a469c9099174b7284de36705ed2bba2e8e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274467"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let contentType = await client.api('/sites/{site-id}/contentTypes/{contentType-id}')
    .version('beta')
    .get();

```