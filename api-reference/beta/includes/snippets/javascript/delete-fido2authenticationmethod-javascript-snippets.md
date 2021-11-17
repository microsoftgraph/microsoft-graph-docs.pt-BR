---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 542070510ed77999e96940312754366ceb1d1b514796789bc40050ef1a018279
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/kim@contoso.com/authentication/fido2Methods/_jpuR-TGZtk6aQCLF3BQjA2')
    .version('beta')
    .delete();

```