---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 92306412c452da5160def384d392810a8cb136be
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/send')
    .post();

```