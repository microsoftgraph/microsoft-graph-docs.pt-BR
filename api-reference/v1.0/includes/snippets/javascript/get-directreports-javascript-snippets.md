---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3afe9d25621418629b7c67b7eabac6ddb18a63dcc1f2596d97978e8b635bc3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160010"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let directReports = await client.api('/me/directReports')
    .get();

```