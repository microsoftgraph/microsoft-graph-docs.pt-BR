---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 91dbcaff05b9781f0970189bfa6a94c8a1a2d29f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981872"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.users("047dd774-f1c4-40f2-82f0-278de79f9b83")
    .reprocessLicenseAssignment()
    .buildRequest()
    .post();

```