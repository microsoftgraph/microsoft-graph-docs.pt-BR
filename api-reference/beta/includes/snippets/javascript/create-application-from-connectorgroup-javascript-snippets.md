---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69104d126c53cf469c83a4aba701dc43ec0e0e47e910534b3e8faed9e51ef2d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327086"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  '@odata.id': 'https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}'
};

await client.api('/applications/{id}/connectorGroup/$ref')
    .version('beta')
    .put(connectorGroup);

```