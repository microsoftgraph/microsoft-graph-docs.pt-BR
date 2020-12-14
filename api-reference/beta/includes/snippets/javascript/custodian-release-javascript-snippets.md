---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 658092ff9f764c2fc98a43a1d4454b73b3f8f2ce
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658950"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/compliance/ediscovery/cases/2192ca408ea2410eba3bec8ae873be6b/custodians/45454331323337443946343043464239/release')
    .version('beta')
    .post();

```