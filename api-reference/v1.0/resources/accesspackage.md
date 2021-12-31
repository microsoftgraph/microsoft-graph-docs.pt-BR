---
title: Tipo de recurso accessPackage
description: Um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 226715a4678b593e68a8364e326950c7af019212
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651453"
---
# <a name="accesspackage-resource-type"></a>Tipo de recurso accessPackage

Namespace: microsoft.graph

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), um pacote de acesso define as coleções de funções de recurso e as políticas de como um ou mais usuários podem obter acesso a esses recursos.  

Cada pacote de acesso é referenciado por um catálogo de pacotes de acesso único e tem links para os recursos desse catálogo por meio dos escopos de função específicos do recurso que definem o acesso que o pacote fornece.  Um pacote de acesso também se vincula às políticas de atribuição de pacote de acesso, cada uma das quais define quem pode solicitar ou ser atribuído a uma atribuição de pacote de acesso.



## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessPackages](../api/entitlementmanagement-list-accesspackages.md)|[Coleção accessPackage](accesspackage.md)|Recupere uma lista de **objetos accesspackage.** |
|[Criar accessPackage](../api/entitlementmanagement-post-accesspackages.md)|[accessPackage](accesspackage.md)|Crie um novo **objeto accesspackage.** |
|[Obter accessPackage](../api/accesspackage-get.md)|[accessPackage](accesspackage.md)|Ler propriedades e relações de um **objeto accesspackage.** |
|[Atualizar accessPackage](../api/accesspackage-update.md)|Nenhum|Atualize as propriedades de um **objeto accesspackage.** |
|[Excluir accessPackage](../api/accesspackage-delete.md)|Nenhum|Excluir um **accesspackage**. |
|[filterByCurrentUser](../api/accesspackage-filterbycurrentuser.md)|[Coleção accessPackage](../resources/accesspackage.md)|Recupere a lista de **objetos accessPackage** filtrados no usuário de entrada.|
|[getApplicablePolicyRequirements](../api/accesspackage-getapplicablepolicyrequirements.md)|[coleção accessPackageAssignmentRequestRequirements](../resources/accesspackageassignmentrequestrequirements.md)|Recupere uma lista de **objetos accessPackageAssignmentRequestRequirement** com requisitos de solicitação. |

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura.|
|description|String|A descrição do pacote de acesso.|
|displayName|String|O nome de exibição do pacote de acesso. Suporta $filter ( `eq` , `contains` ).|
|id|String|Somente leitura.|
|IsHidden|Booleano|Se o pacote de acesso está oculto do solicitante.|
|modifiedDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Somente leitura. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|catalog|[accessPackageCatalog](../resources/accesspackagecatalog.md)|Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackage",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "isHidden": "Boolean",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```


