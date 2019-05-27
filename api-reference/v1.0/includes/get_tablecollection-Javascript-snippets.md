---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fad18d05eb54efd0dfa2e4ab46c120f6bbe942c8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481160"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables')
    .get();

```