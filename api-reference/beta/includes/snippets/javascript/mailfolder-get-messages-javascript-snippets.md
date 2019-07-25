---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 312571136d5e162797d53ffa969b7204c9cf08dc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35879992"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/mailFolders/AAMkAGVmMDEzM/messages')
    .version('beta')
    .get();

```