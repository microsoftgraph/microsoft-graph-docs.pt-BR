---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 019a4c99e95de4bd16e6695fe3506994df3bbfe53a9f8aca470728630d68020a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let credentialUserRegistrationsSummary = await client.api('/tenantRelationships/managedTenants/credentialUserRegistrationsSummaries/{credentialUserRegistrationsSummaryId}')
    .version('beta')
    .get();

```