---
title: tipo de recurso connectedOrganization
description: No Azure AD pretitulation Management, uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.
author: markwahl-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f5d53e3a24ad8e99c22d61bc6a4d519888c4aafd
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/29/2020
ms.locfileid: "47311287"
---
# <a name="connectedorganization-resource-type"></a>tipo de recurso connectedOrganization

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar connectedOrganizations](../api/connectedorganization-list.md) | coleção [connectedOrganization](connectedorganization.md) | Recupere uma lista de objetos connectedOrganization. |
|[Criar connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | Criar um novo objeto connectedOrganization. |
|[Obter connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Ler propriedades e relações de um objeto connectedOrganization. |
|[Atualizar connectedOrganization](../api/connectedorganization-update.md) | | Atualizar um connectedOrganization. |
|[Excluir connectedOrganization](../api/connectedorganization-delete.md) |Nenhum | Excluir um connectedOrganization. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de patrocinadores internos de um connectedOrganization. |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de patrocinadores externos de um connectedOrganization. |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Nenhum | Adicionar um usuário ou grupo aos patrocinadores internos de um connectedOrganization. |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Nenhum | Adicionar um usuário ou grupo aos patrocinadores externos de um connectedOrganization. |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Nenhum | Remover um usuário ou grupo dos patrocinadores internos de um connectedOrganization. |
|[Remover externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Nenhum | Remover um usuário ou grupo dos patrocinadores externos de um connectedOrganization. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|String|UPN do usuário que criou este recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|description|String|A descrição da organização conectada.|
|displayName|String|O nome de exibição da organização conectada.|
|id|String| Somente leitura.|
|modifiedBy|String|UPN do usuário que modificou este recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Somente leitura.|
|state|connectedOrganizationState|O estado de uma organização conectada define se as políticas de atribuição com tipo de escopo solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não. Os valores possíveis são: `configured`, `proposed`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|identitySources|coleção [identityry](identitySource.md)| As fontes de identidade nesta organização conectada, uma de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md). Somente leitura. Anulável.|
|internalSponsors| Coleção [directoryObject](directoryobject.md)| Anulável.|
|externalSponsors| Coleção [directoryObject](directoryobject.md)| Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
      "tenantId": "String (identifier)",
      "displayName": "String"
    }
  ],
  "state": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
