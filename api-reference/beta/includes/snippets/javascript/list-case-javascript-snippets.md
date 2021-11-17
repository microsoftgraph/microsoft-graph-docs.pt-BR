---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af0c390b55aecc1e74560b8230ff2e4d082a6117964229f84463f7090c586da1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101611"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cases = await client.api('/compliance/ediscovery/cases')
    .version('beta')
    .get();

```