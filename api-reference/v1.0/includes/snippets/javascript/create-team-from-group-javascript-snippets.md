---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0fb1d9dd8c7c90231340d5378bad44fd29d666c
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374033"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  group@odata.bind: "https://graph.microsoft.com/v1.0/groups('groupId')"
};

let res = await client.api('/teams')
    .post(team);

```