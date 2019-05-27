---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 262e2df8e69c4fef0aa6fff002e35df034ea6c47
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434271"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/delta')
    .header('Prefer','return=minimal')
    .select('displayName,jobTitle,mobilePhone')
    .get();

```