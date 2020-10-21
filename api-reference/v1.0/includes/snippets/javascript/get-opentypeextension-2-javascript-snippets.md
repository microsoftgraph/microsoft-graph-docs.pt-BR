---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 172ceac6d0df77d4e543983ff54e5b4d58d8f585
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609292"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/f5480dfd-7d77-4d0b-ba2e-3391953cc74a/events/AAMkADVl17IsAAA=/extensions/Com.Contoso.Deal/')
    .get();

```