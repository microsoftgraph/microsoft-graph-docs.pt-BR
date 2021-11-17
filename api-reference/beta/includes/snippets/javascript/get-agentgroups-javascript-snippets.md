---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c85e925cce9025d203411ba2707469df72001314473dd1bc5c48b7dd425dcd9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326722"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let agentGroups = await client.api('/onPremisesPublishingProfiles/provisioning/agentGroups')
    .version('beta')
    .expand('publishedResources')
    .get();

```