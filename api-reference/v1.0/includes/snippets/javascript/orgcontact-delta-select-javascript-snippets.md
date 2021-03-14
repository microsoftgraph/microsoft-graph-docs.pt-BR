---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dbdff29d2b101b679b0b0a8e4d24f4f24397d32b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795023"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/contacts/delta')
    .select('displayName,jobTitle,mail')
    .get();

```