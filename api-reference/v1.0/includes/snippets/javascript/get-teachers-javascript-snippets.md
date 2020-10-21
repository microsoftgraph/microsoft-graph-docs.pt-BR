---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94ab6ac29d87b9e61f0cdb8ab73cf65c0710176a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611706"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/education/classes/{class-id}/teachers')
    .get();

```