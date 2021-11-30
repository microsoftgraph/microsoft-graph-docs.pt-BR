---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b884920ac8f974c5317d10d3ab8df4e3df19fd21
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224089"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
    securityEnabledOnly: false
};

await client.api('/directoryObjects/0049d944-a805-4680-9f54-3ab292090309/getMemberGroups')
    .post(string);

```