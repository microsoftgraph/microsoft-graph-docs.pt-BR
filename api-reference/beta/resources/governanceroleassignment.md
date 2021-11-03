---
title: Tipo de recurso governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: 424357bdef9915347eaa99478d434a4e1ea39d02
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696417"
---
# <a name="governanceroleassignment-resource-type"></a>Tipo de recurso governanceRoleAssignment

Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1resourceroles-deprecation](../../includes/pim-v1resourceroles-deprecation.md)]

Representa a atribuição de um usuário ou grupo a uma função.

Privileged Identity Management (PIM) oferece suporte a dois tipos de atribuições:

1. Atribuição ativa - Representa o acesso direto/ativado aos recursos.
2. Atribuição qualificada - representa um estágio intermediário de acesso privilegiado a recursos, entre nenhum acesso e acesso direto. Os administradores podem atribuir usuários/grupos com antecedência e, sempre que o acesso for necessário, o acesso é necessário para obter o acesso instantâneo ao recurso `eligible assignment` `activation` por várias `eligible assignment` horas. Após a ativação, `active assignment` um será criado para os usuários/membros do grupo indicarem o status ativado.

## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Ler propriedades e relações de uma entidade de atribuição de função.|
|[Lista](../api/governanceroleassignment-list.md) | [Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)|Listar uma coleção de atribuições de função em um recurso. |
|[Export](../api/governanceroleassignment-export.md) | octet-stream |Baixe uma coleção de atribuições de função em um recurso e salve como um `.csv` arquivo.|

Não `POST` , , ou as operações são `PUT` `PATCH` `DELETE` suportadas no conjunto de `roleAssignments` entidades. Todas as operações de criação, atualização e exclusão são `governanceRoleAssignment` feitas por `governanceRoleAssignmentRequest` .

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |String     |A ID da atribuição de função. Está no formato GUID.|
|resourceId |String     |Obrigatório. A ID do recurso ao qual a atribuição de função está associada. |
|roleDefinitionId|String|Obrigatório. A ID da definição de função à qual a atribuição de função está associada. |
|subjectId|String       |Obrigatório. A ID do assunto ao qual a atribuição de função está associada. |
|linkedEligibleRoleAssignmentId|String|Se for um e criado devido à `active assignment` ativação em `eligible assignment` um , ele representará a ID `eligible assignment` disso; Caso contrário, o valor será `null` . |
|externalId   |Cadeia de caracteres     |A ID externa do recurso usado para identificar a atribuição de função no provedor.|
|startDateTime|DateTimeOffset|A hora de início da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|Para uma atribuição de função não permanente, este é o momento em que a atribuição de função será expirada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|assignmentState|String  |O estado da atribuição. O valor pode ser para atribuição qualificada ou se ele for atribuído diretamente pelos administradores ou ativado em uma atribuição qualificada `Eligible` `Active` pelos `Active` usuários.|
|memberType|String      |O tipo de membro. O valor pode ser: (se a atribuição de função for herdada de um escopo de recurso pai), (se a atribuição de função não for herdada, mas vier da associação de uma atribuição de grupo) ou (se a atribuição de função não for herdada nem de uma atribuição de `Inherited` `Group` `User` grupo).|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Apenas leitura. O recurso associado à atribuição de função. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Apenas leitura. A definição de função associada à atribuição de função. |
|assunto|[governanceSubject](../resources/governancesubject.md)|Apenas leitura. O assunto associado à atribuição de função. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Apenas leitura. Se for um `active assignment` e criado devido à ativação em um , ele `eligible assignment` representará o objeto disso `eligible assignment` ; Caso contrário, o valor será `null` . |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceRoleAssignment"
}-->

```json
{
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "subjectId": "String",
  "linkedEligibleRoleAssignmentId": "String",
  "externalId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "assignmentState": "String",
  "memberType": "String",
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


