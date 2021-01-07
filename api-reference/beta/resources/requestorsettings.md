---
title: tipo complexo requestorSettings
description: Usada para a `requestorSettings` propriedade de uma política de atribuição de pacote do Access. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ccaa57a3dfa2f81d33e4e6fea804a91d1db7da20
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777607"
---
# <a name="requestorsettings-resource-type"></a>tipo de recurso requestorSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a propriedade **requestorSettings** de uma [política de atribuição de pacote do Access](accesspackageassignmentpolicy.md). Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote do Access nessa política.

| Quem pode solicitar | scopeType | coleção allowedRequestors|
|:----------------|:----------|:------------------|
|Ninguém|`NoSubjects`|matriz vazia|
|Usuário individual específico em seu diretório|`SpecificDirectorySubjects`|[Únicousuário](singleuser.md)|
|Usuários em seu diretório que são membros de um grupo|`SpecificDirectorySubjects`|[groupMembers](groupmembers.md)|
|Os usuários em seu diretório com o `userType` valor de `member`|`AllExistingDirectoryMemberUsers`|matriz vazia|
|Usuários no seu diretório|`AllExistingDirectorySubjects`|matriz vazia|
|Usuários em organizações conectadas específicas|`SpecificConnectedOrganizationSubjects`|[connectedOrganizationMembers](connectedorganizationmembers.md)|
|Usuários de todas as organizações conectadas que têm a propriedade State da organização conectada definida como `configured` .|`AllConfiguredConnectedOrganizationSubjects`|matriz vazia|
|Qualquer usuário|`AllExternalSubjects`|matriz vazia|

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |Cadeia de caracteres |Quem pode solicitar. Um dos `NoSubjects` , `SpecificDirectorySubjects` , `SpecificConnectedOrganizationSubjects` , `AllConfiguredConnectedOrganizationSubjects` , `AllExistingConnectedOrganizationSubjects` , `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` ou `AllExternalSubjects` .  |
| acceptRequests | Booliano | Indica se novas solicitações serão aceitas nessa política. |
| allowedRequestors | coleção [userset](userset.md)| Os usuários que têm permissão para solicitar essa política, que podem ser [únicousuário](singleuser.md), [groupMembers](groupmembers.md)e [connectedOrganizationMembers](connectedorganizationmembers.md). |

## <a name="json-representation"></a>Representação JSON


Veja a seguir uma representação JSON da propriedade **requestorSettings** de uma política, que permite aos membros de um grupo solicitar.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requestorSettings"
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


