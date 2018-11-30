---
title: tipo de recurso de governanceRoleDefinition
description: Representa as definições de função. Para obter recursos Azure, ela pode representar funções de RBAC do Azure, proprietário, leitor, colaborador, etc.
ms.openlocfilehash: 057d74276b41abad47eb60ce48a99f1160c401ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034777"
---
# <a name="governanceroledefinition-resource-type"></a>tipo de recurso de governanceRoleDefinition

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção. 


Representa as definições de função. Para obter recursos Azure, ela pode representar funções de RBAC do Azure, proprietário, leitor, colaborador, etc.


## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:---------------|:--------|:--------|:----------|
|[List](../api/governanceroledefinition-list.md) | coleção [governanceRoleDefinition](../resources/governanceroledefinition.md) |Uma coleção de definições de função em um recurso de lista.|
|[Get](../api/governanceroledefinition-get.md) | [governanceRoleDefinition](../resources/governanceroledefinition.md) |Leia as propriedades e os relacionamentos de uma entidade de definição de função especificado pelo id.|
Não `POST`, `PUT`, `PATCH`, `DELETE` tem suporte nos `roleDefinitions` conjunto de entidade para agora.
## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----|:----------|:----------|:----------|
|id         |String     |A id da definição de função. |
|resourceId |Cadeia de caracteres     |Obrigatório. A identificação do recurso associado à definição de função. |
|externalId   |Cadeia de caracteres     |A id externa da definição de função.|
|displayName|String     |O nome de exibição da definição de função.|
|subjectCount|Int32     |Opcional. O número de assuntos que são atribuídas à função. Representa o status de acesso do solicitador para o recurso. Para obter a propriedade, faça uso explicitamente `$select=subjectCount` na consulta.|
|eligibleAssignmentCount|Int32|Opcional. O número de atribuições de função elegíveis associado à definição de função. Para obter a propriedade, faça uso explicitamente `$select=eligibleAssignmentCount` na consulta.|
|activeAssignmentCount|Int32    |Opcional. O número de atribuições de função ativa associado à definição de função.  Para obter a propriedade, faça uso explicitamente `$select=activeAssignmentCount` na consulta.|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado para a definição de função.|
|roleSetting|[governanceRoleSetting](../resources/governancerolesetting.md)|A configuração da função associada para a definição de função.|

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->