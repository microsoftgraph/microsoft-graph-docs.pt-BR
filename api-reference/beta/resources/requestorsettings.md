---
title: tipo complexo requestorSettings
description: Usada para a `requestorSettings` propriedade de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b52f3276185f819ccd0e7149dbd5420b4f6e1781
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521114"
---
# <a name="requestorsettings-resource-type"></a>tipo de recurso requestorSettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a propriedade **requestorSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote do Access nessa política.

| Quem pode solicitar | scopeType | coleção allowedRequestors|
|:----------------|:----------|:------------------|
|Ninguém|`NoSubjects`|matriz vazia|
|Usuário individual específico em seu diretório|`SpecificDirectorySubjects`|[Únicousuário](singleuser.md)|
|Usuários em seu diretório que são membros de um grupo|`SpecificDirectorySubjects`|[groupMembers](groupmembers.md)|
|Os usuários em seu diretório `userType` com o valor de`member`|`AllExistingDirectoryMemberUsers`|matriz vazia|
|Usuários no seu diretório|`AllExistingDirectorySubjects`|matriz vazia|
|Usuários em outras organizações conectadas já configuradas|`SpecificConnectedOrganizationSubjects`|[connectedOrganizationMembers](connectedorganizationmembers.md)|
|Usuários de outras organizações conectadas já configuradas|`AllExistingConnectedOrganizationSubjects`|matriz vazia|
|Qualquer usuário|`AllExternalSubjects`|matriz vazia|

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |String |Quem pode solicitar. Um dos `NoSubjects`, `SpecificDirectorySubjects`, `SpecificConnectedOrganizationSubjects`, `AllExistingConnectedOrganizationSubjects`, `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` ou `AllExternalSubjects`.  |
| acceptRequests | Boolean | Indica se novas solicitações serão aceitas nessa política. |
| allowedRequestors | coleção [userset](userset.md)| Os usuários que têm permissão para solicitar essa política, que podem ser [únicousuário](singleuser.md), [groupMembers](groupmembers.md)e [connectedOrganizationMembers](connectedorganizationmembers.md). |

## <a name="json-representation"></a>Representação JSON


Veja a seguir uma representação JSON da propriedade **requestorSettings** de uma política, que permite aos membros de um grupo solicitar.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings",
  "baseType": ""
}-->

```json
{
  "scopeType": "SpecificDirectorySubjects",
  "acceptRequests": true,
  "allowedRequestors": [
       {
         "@odata.type": "#microsoft.graph.groupMembers",
         "isBackup": false,
         "id": "string (identifier)",
         "description": "Authorized requestors"
       }
   ]
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "requestorSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
