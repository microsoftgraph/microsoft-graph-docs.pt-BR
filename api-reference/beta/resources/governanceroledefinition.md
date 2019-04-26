---
title: tipo de recurso governanceRoleDefinition
description: Representa as definições de função. Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.
localization_priority: Normal
ms.openlocfilehash: 867864892bac9107c44ba9125336429248b6697e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547437"
---
# <a name="governanceroledefinition-resource-type"></a>tipo de recurso governanceRoleDefinition

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]


Representa as definições de função. Para os recursos do Azure, ele pode representar as funções do Azure RBAC, como proprietário, leitor, colaborador, etc.


## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | coleção [governanceRoleDefinition](../resources/governanceroledefinition.md) |Lista uma coleção de definições de função em um recurso.|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Ler propriedades e relações de uma entidade de definição de função especificado por ID.|
Não `POST`, `PUT`, `PATCH`, `DELETE` tem suporte no `roleDefinitions` conjunto de entidades por enquanto.
## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----|:----------|:----------|:----------|
|id         |String     |A ID da definição de função. |
|resourceId |String     |Obrigatório. A ID do recurso associada à definição de função. |
|externalId   |Cadeia de caracteres     |A ID externa da definição de função.|
|displayName|String     |O nome de exibição da definição de função.|
|subjectCount|Int32     |Opcional. O número de entidades atribuídas à função. Ele representa o status do acesso do solicitante ao recurso. Para obter a propriedade, explictly use `$select=subjectCount` na consulta.|
|eligibleAssignmentCount|Int32|Opcional. O número de atribuições de função qualificadas associadas à definição de função. Para obter a propriedade, explictly use `$select=eligibleAssignmentCount` na consulta.|
|activeAssignmentCount|Int32    |Opcional. O número de atribuições de função ativas associadas à definição de função.  Para obter a propriedade, explictly use `$select=activeAssignmentCount` na consulta.|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[Entidadegovernanceresource](../resources/governanceresource.md)|Somente leitura. O recurso associado para a definição de função.|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|A configuração de função associada para a definição de função.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "externalId": "String",
  "displayName": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroledefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
