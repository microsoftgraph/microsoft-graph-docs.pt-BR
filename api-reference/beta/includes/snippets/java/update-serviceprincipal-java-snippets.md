---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 066e164aabdd71f2969d34768da1eaeef9aa0d9d
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35869879"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipal servicePrincipal = new ServicePrincipal();
servicePrincipal.accountEnabled = true;
LinkedList<AddIn> addInsList = new LinkedList<AddIn>();
AddIn addIns = new AddIn();
addIns.id = "id-value";
addIns.type = "type-value";
LinkedList<KeyValue> propertiesList = new LinkedList<KeyValue>();
KeyValue properties = new KeyValue();
properties.key = "key-value";
properties.value = "value-value";
propertiesList.add(properties);
addIns.properties = propertiesList;
addInsList.add(addIns);
servicePrincipal.addIns = addInsList;
servicePrincipal.appDisplayName = "appDisplayName-value";
servicePrincipal.appId = "appId-value";
servicePrincipal.appOwnerOrganizationId = "appOwnerOrganizationId-value";
servicePrincipal.appRoleAssignmentRequired = true;

graphClient.servicePrincipals("{id}")
    .buildRequest()
    .patch(servicePrincipal);

```