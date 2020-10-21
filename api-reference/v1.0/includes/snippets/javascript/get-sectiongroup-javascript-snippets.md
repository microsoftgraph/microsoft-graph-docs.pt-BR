---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d1920047e3c36c8f6a2110446cd6bdbd604cc47
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604888"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}')
    .get();

```