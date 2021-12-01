---
title: Tipo de recurso connectedOrganization
description: No gerenciamento de direitos do Azure AD, uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 42ec49fd292f0e7c59002a57f7f4ccaff47c292d
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242241"
---
# <a name="connectedorganization-resource-type"></a>Tipo de recurso connectedOrganization

Namespace: microsoft.graph


No gerenciamento de direitos do [Azure AD,](entitlementmanagement-root.md)uma organização conectada é uma referência a um diretório ou domínio de outra organização cujos usuários podem solicitar acesso.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar connectedOrganizations](../api/entitlementmanagement-list-connectedorganizations.md)|[Coleção connectedOrganization](connectedorganization.md)|Recupere uma lista de objetos connectedOrganization. |
|[Criar connectedOrganization](../api/entitlementmanagement-post-connectedorganizations.md)|[connectedOrganization](connectedorganization.md)|Crie um novo objeto connectedOrganization. |
|[Obter connectedOrganization](../api/connectedorganization-get.md)|[connectedOrganization](connectedorganization.md)|Leia propriedades e relações de um objeto connectedOrganization. |
|[Atualizar connectedOrganization](../api/connectedorganization-update.md)|[Coleção connectedOrganization](connectedorganization.md)|Atualize uma connectedOrganization. |
|[Excluir connectedOrganization](../api/connectedorganization-delete.md)|Nenhum|Excluir uma connectedOrganization. |
|[Listar externalSponsors](../api/connectedorganization-list-externalsponsors.md)|Coleção [directoryObject](directoryobject.md)|Recupere uma lista de patrocinadores externos de uma connectedOrganization. |
|[Adicionar externalSponsors](../api/connectedorganization-post-externalsponsors.md)|Nenhum|Adicione um usuário ou grupo aos patrocinadores externos de um connectedOrganization. |
|[Listar internalSponsors](../api/connectedorganization-list-internalsponsors.md)|Coleção [directoryObject](directoryobject.md)|Recupere uma lista dos patrocinadores internos de uma connectedOrganization. |
|[Adicionar internalSponsors](../api/connectedorganization-post-internalsponsors.md)|Nenhum|Adicione um usuário ou grupo aos patrocinadores internos de um connectedOrganization. |
|[Remover internalSponsors](../api/connectedorganization-delete-internalsponsors.md)|Nenhum|Remova um usuário ou grupo dos patrocinadores internos do connectedOrganization. |
|[Remover externalSponsors](../api/connectedorganization-delete-externalsponsors.md)|Nenhum|Remova um usuário ou grupo dos patrocinadores externos do connectedOrganization. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|Cadeia de caracteres|A descrição da organização conectada.|
|displayName|Cadeia de caracteres|O nome de exibição da organização conectada.|
|id|String|Somente leitura.|
|identitySources|[Coleção identitySource](../resources/identitysource.md)|As fontes de identidade nesta organização conectada, uma de [azureActiveDirectoryTenant](azureactivedirectorytenant.md), [domainIdentitySource](domainidentitysource.md) ou [externalDomainFederation](externaldomainfederation.md). Anulável.|
|modifiedDateTime|DateTimeOffset|*O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|state|connectedOrganizationState|O estado de uma organização conectada define se as políticas de atribuição com o tipo de escopo do solicitante `AllConfiguredConnectedOrganizationSubjects` são aplicáveis ou não.  Os valores possíveis são: `configured`, `proposed`, `unknownFutureValue`.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|externalSponsors|Coleção [directoryObject](directoryobject.md)|Anulável.|
|internalSponsors|Coleção [directoryObject](directoryobject.md)|Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.connectedOrganization",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.connectedOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "identitySources": [
    {
      "@odata.type": "microsoft.graph.azureActiveDirectoryTenant"
    }
  ],
  "state": "String"
}
```


