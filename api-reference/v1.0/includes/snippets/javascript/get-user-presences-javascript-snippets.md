---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b16ab641031e491f9b6b648a6744d4d981e204bc
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/communications/presences/dc74d9bb-6afe-433d-8eaa-e39d80d3a647')
    .get();

```