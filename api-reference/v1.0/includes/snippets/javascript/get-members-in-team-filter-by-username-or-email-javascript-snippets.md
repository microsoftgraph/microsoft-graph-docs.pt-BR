---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8a8cca45637848ffbf656825ab3d9183d67f02cf9e0109c800133a68a79b3c0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213906"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .filter('(microsoft.graph.aadUserConversationMember/displayName eq \'Harry Johnson\' or microsoft.graph.aadUserConversationMember/email eq \'admin@M365x987948.OnMicrosoft.com\')')
    .get();

```