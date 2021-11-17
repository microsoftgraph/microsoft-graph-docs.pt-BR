---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60628bd303e0ff182b0798646502d3292512a0d314f741a3743157479275b9cd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let windowsHelloForBusinessAuthenticationMethod = await client.api('/users/annie@contoso.com/authentication/windowsHelloForBusinessMethods/_jpuR-TGZtk6aQCLF3BQjA2')
    .version('beta')
    .get();

```