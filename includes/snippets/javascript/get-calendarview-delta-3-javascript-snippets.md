---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a70d8a20232feeed475e8ef9a1bbc11c1b1492f9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/calendarView/delta')
    .header('Prefer','odata.maxpagesize=2')
    .skiptoken('R0usmci39OQxqJrxK4')
    .get();

```