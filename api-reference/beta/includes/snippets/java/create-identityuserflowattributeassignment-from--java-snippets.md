---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06abb120eb55090cb76ec8fdfc2471ca197f4bbc
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689500"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IdentityUserFlowAttributeAssignment identityUserFlowAttributeAssignment = new IdentityUserFlowAttributeAssignment();
identityUserFlowAttributeAssignment.isOptional = false;
identityUserFlowAttributeAssignment.requiresVerification = false;
identityUserFlowAttributeAssignment.userInputType = IdentityUserFlowAttributeInputType.TEXT_BOX;
identityUserFlowAttributeAssignment.displayName = "Shoe size";
LinkedList<UserAttributeValuesItem> userAttributeValuesList = new LinkedList<UserAttributeValuesItem>();
identityUserFlowAttributeAssignment.userAttributeValues = userAttributeValuesList;
IdentityUserFlowAttribute userAttribute = new IdentityUserFlowAttribute();
userAttribute.id = "extension_guid_shoeSize";
identityUserFlowAttributeAssignment.userAttribute = userAttribute;

graphClient.identity().b2xUserFlows("B2X_1_Partner").userAttributeAssignments()
    .buildRequest()
    .post(identityUserFlowAttributeAssignment);

```