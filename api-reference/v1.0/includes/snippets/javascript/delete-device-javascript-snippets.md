---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97c255c7140f46aa8f99c1d79a31d461db79b38c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices/{id}')
    .delete();

```