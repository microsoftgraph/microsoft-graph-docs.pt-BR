---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04466d1255bfa40996d6d1cef861a1d6baea4902
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43510514"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/applications/{id}/tokenLifetimePolicies')
    .get();

```