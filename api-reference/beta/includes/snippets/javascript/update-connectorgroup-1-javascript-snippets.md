---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 57dda30263ce534f3d9e9b911b650630f5d3cc746c70e874105dff214466c5a4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectorGroup = {
  name: 'Connector Group Demo'

};

await client.api('/onPremisesPublishingProfiles/applicationProxy/connectorGroups')
    .version('beta')
    .post(connectorGroup);

```