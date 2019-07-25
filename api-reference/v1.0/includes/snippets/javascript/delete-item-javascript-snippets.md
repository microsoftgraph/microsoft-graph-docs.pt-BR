---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 743f327c4adaef1f47eddc4d218f8335eb08bb17
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35894769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}')
    .delete();

```