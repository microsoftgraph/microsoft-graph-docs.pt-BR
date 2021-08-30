---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa0564d6892ffc9bb70dbbbcec22067fc27ff12b98b5ca38b7e7a116f62dd878
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let members = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .version('beta')
    .filter('(microsoft.graph.aadUserConversationMember/displayName eq \'Harry Johnson\' or microsoft.graph.aadUserConversationMember/email eq \'admin@M365x987948.OnMicrosoft.com\')')
    .get();

```