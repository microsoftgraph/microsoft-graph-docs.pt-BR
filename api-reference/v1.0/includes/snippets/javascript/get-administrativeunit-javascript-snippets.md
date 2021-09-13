---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a595451a18ffdf056a601e7e7cb50bc016eb8b90c89f20f989b29c00c1e2183d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329774"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let administrativeUnit = await client.api('/directory/administrativeUnits/{id}')
    .get();

```