---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d79b81b03759afffebb06c1848a648ccc616fa529bac93c191b76dc0d7b90218
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalConnection = {
  id: 'contosohr',
  name: 'Contoso HR',
  description: 'Connection to index Contoso HR system'
};

await client.api('/external/connections')
    .post(externalConnection);

```