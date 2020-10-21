---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b7fb9addbfb14c0b3016b2916ac5092b5d21f15f
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoleTemplates/{id}')
    .get();

```