---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 72cbfb54f9b71e6a97adae46b147d6e6be7e4e062534329d7609eee9706ab5b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/schools/delta')
    .version('beta')
    .get();

```