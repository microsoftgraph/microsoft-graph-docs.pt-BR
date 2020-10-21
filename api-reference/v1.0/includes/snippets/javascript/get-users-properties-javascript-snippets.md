---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 74d8efe099cf1a3d7f8fe5423a78577e1a7c5f68
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48613861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users')
    .select('displayName,givenName,postalCode')
    .get();

```