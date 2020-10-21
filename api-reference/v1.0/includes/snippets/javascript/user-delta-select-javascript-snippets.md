---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 29663036263e53dd35b20c5575424959a7c665b1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607479"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```