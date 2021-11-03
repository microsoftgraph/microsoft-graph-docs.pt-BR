---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab179a01b0247a5f3515191707fe6abc4127760002ed443e97a56e62339ad4f4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

BookingStaffMember bookingStaffMember = graphClient.bookingBusinesses("Contosolunchdelivery@M365B489948.onmicrosoft.com").staffMembers("71d64d0e-7225-49b6-b0b1-070d476cda51")
    .buildRequest()
    .get();

```