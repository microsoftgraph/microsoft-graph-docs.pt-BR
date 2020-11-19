---
description: Automatically generated file. DO NOT MODIFY
ms.openlocfilehash: 5bd1f71c29b44c6443d60c9b0fc1a24ee84847f3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221993"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/pendingAccessReviewInstances')
    .version('beta')
    .expand('definition')
    .skip(0)
    .top(100)
    .get();

```