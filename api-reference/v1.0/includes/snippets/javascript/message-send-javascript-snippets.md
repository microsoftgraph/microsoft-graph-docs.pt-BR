---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92306412c452da5160def384d392810a8cb136be
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731937"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/send')
    .post();

```