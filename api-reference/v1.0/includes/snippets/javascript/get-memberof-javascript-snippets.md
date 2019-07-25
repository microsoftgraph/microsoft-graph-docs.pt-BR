---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad619386e45e976e531b7bec7ac9f69b7070202d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894814"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/memberOf')
    .get();

```