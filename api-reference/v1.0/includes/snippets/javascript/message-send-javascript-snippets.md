---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92306412c452da5160def384d392810a8cb136be
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/send')
    .post();

```