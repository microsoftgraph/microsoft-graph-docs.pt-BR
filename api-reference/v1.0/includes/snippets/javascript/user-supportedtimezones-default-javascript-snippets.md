---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4fba4fd09f7eb899617f79887a0feb1d2483184
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612208"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/supportedTimeZones')
    .get();

```