---
title: Tipo complexo requestorSettings
description: Usado para a propriedade `requestorSettings` de uma política de atribuição de pacote de acesso. Fornece configurações adicionais para selecionar quem pode criar uma solicitação.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a9bd91605d106b488de21f29baefe4b31d28f323
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133725"
---
# <a name="requestorsettings-resource-type"></a>Tipo de recurso requestorSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Usado para a **propriedade requestorSettings** de uma política [de atribuição de pacote de acesso.](accesspackageassignmentpolicy.md) Fornece configurações adicionais para selecionar quem pode criar uma solicitação para um pacote de acesso nessa política.

| Quem pode solicitar | scopeType | Coleção allowedRequestors|
|:----------------|:----------|:------------------|
|Ninguém|`NoSubjects`|matriz vazia|
|Usuário individual específico em seu diretório|`SpecificDirectorySubjects`|[singleUser](singleuser.md)|
|Usuários em seu diretório que são membros de um grupo|`SpecificDirectorySubjects`|[groupMembers](groupmembers.md)|
|Usuários em seu diretório com `userType` valor de `member`|`AllExistingDirectoryMemberUsers`|matriz vazia|
|Usuários em seu diretório|`AllExistingDirectorySubjects`|matriz vazia|
|Usuários em organizações conectadas específicas|`SpecificConnectedOrganizationSubjects`|[connectedOrganizationMembers](connectedorganizationmembers.md)|
|Usuários de qualquer organização conectada que tenham a propriedade de estado da organização conectada definida como `configured` .|`AllConfiguredConnectedOrganizationSubjects`|matriz vazia|
|Qualquer usuário|`AllExternalSubjects`|matriz vazia|

## <a name="properties"></a>Propriedades

| Propriedade                     | Tipo                      | Descrição |
| :--------------------------- | :------------------------ | :---------- |
| scopeType |String |Quem pode solicitar. Um de `NoSubjects` , , , , ou `SpecificDirectorySubjects` `SpecificConnectedOrganizationSubjects` `AllConfiguredConnectedOrganizationSubjects` `AllExistingConnectedOrganizationSubjects` `AllExistingDirectoryMemberUsers` `AllExistingDirectorySubjects` `AllExternalSubjects` .  |
| acceptRequests | Boolean | Indica se novas solicitações são aceitas nesta política. |
| allowedRequestors | [Coleção userSet](userset.md)| Os usuários que têm permissão para solicitar nesta política, que pode ser [singleUser](singleuser.md), [groupMembers](groupmembers.md)e [connectedOrganizationMembers](connectedorganizationmembers.md). |

## <a name="json-representation"></a>Representação JSON


A seguir está uma representação JSON da **propriedade requestorSettings** de uma política, que permite que os membros de um grupo solicitem.

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


