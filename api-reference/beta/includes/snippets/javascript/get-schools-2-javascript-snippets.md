---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 672837636103f43f5f22e8ac13237bbebb2103e3471c4463694d68e9ed9fd847
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let schools = await client.api('/education/schools')
    .version('beta')
    .get();

```