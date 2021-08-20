---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef21d86abbd593ca578059e9f75342eff8fc20ce
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58264162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let serviceHealth = await client.api('/admin/serviceAnnouncement/healthOverviews/Microsoft 365 suite')
    .expand('issues')
    .get();

```