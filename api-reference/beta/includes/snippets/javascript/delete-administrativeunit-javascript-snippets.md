---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa0802b4538a1d8b893cd9db7164a1295134cef684e11683494153065809f35f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099756"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/administrativeUnits/{id}')
    .version('beta')
    .delete();

```