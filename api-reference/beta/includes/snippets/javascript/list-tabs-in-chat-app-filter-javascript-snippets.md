---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12d5eb330c7102cda1c98b25bdc1f41b18683c5262f56dd27ce81d16ebbc6f93
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tabs = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .filter('teamsApp/id eq \'com.microsoft.teamspace.tab.web\'')
    .expand('teamsApp')
    .get();

```