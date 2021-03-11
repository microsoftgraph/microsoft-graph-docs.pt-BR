---
title: Tipo de recurso connectedOrganization
description: No gerenciamento de direitos do Azure AD, uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.
author: markwahl-msft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 01837683481008fa79c2213970404413bdd6efe2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721681"
---
# <a name="connectedorganization-resource-type"></a>Tipo de recurso connectedOrganization

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar connectedOrganizations](../api/connectedorganization-list.md) | [Coleção connectedOrganization](connectedorganization.md) | Recupere uma lista de objetos connectedOrganization. |
|[Criar connectedOrganization](../api/connectedorganization-post.md) | [connectedOrganization](connectedorganization.md) | Crie um novo objeto connectedOrganization. |
|[Obter connectedOrganization](../api/connectedorganization-get.md) | [connectedOrganization](connectedorganization.md) | Leia propriedades e relações de um objeto connectedOrganization. |
|[Atualizar connectedOrganization](../api/connectedorganization-update.md) | | Atualize uma connectedOrganization. |
|[Excluir connectedOrganization](../api/connectedorganization-delete.md) |Nenhum(a) | Excluir uma connectedOrganization. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista dos patrocinadores internos de uma connectedOrganization. |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md) | Coleção [directoryObject](directoryobject.md) | Recupere uma lista de patrocinadores externos de uma connectedOrganization. |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md) | Nenhum(a) | Adicione um usuário ou grupo aos patrocinadores internos de um connectedOrganization. |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md) | Nenhum(a) | Adicione um usuário ou grupo aos patrocinadores externos de um connectedOrganization. |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md) | Nenhum(a) | Remova um usuário ou grupo dos patrocinadores internos de uma connectedOrganization. |
|[Remover externalSponsors](../api/connectedorganization-delete-externalsponsors.md) | Nenhum(a) | Remova um usuário ou grupo dos patrocinadores externos de uma connectedOrganization. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdBy|Cadeia de caracteres|UPN do usuário que criou esse recurso. Somente leitura.|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|Cadeia de caracteres|A descrição da organização conectada.|
|displayName|Cadeia de caracteres|O nome de exibição da organização conectada.|
|id|String| Somente leitura.|
|modifiedBy|Cadeia de caracteres|UPN do usuário que modificou esse recurso pela última vez. Somente leitura.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|state|connectedOrganizationState|O estado de uma organização conectada define se as políticas de atribuição com o tipo de escopo do solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não. Os valores possíveis são: `configured`, `proposed`.|

## <a name="relationships"></a>Relações

|Relação|Tipo|Descrição|
|:---|:---|:---|
|identitySources|[Coleção identitySource](identitySource.md)| As fontes de identidade nesta organização conectada, uma de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md). Somente leitura. Anulável.|
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


