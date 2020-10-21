---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f155d22ffbb26993694d34b9d786e2251730a190
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/events/{id}')
    .delete();

```