---
title: Tipo de recurso governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 76aaa6e63b9c44e1bc3db1ccf6e8351a5796051f
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65399457"
---
# <a name="governanceroleassignment-resource-type"></a>Tipo de recurso governanceRoleAssignment

Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2ResourceRoles-deprecation](../../includes/pim-v2ResourceRoles-deprecation.md)]

Representa a atribuição de um usuário ou grupo a uma função.

Privileged Identity Management (PIM) dá suporte a dois tipos de atribuições:

1. Atribuição ativa – representa o acesso direto/ativado aos recursos.
2. Atribuição qualificada – representa um estágio intermediário de acesso privilegiado a recursos, entre nenhum acesso e acesso direto. Os administradores podem atribuir usuários/`eligible assignment`grupos com antecedência e, sempre que o acesso for necessário, `eligible assignment` `activation` no necessário para obter o acesso instantâneo ao recurso por várias horas. Após a ativação `active assignment` , um será criado para os usuários/membros do grupo indicarem o status ativado.

## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Ler propriedades e relações de uma entidade de atribuição de função.|
|[Listar](../api/governanceroleassignment-list.md) | [coleção governanceRoleAssignment](../resources/governanceroleassignment.md)|Listar uma coleção de atribuições de função em um recurso. |
|[Export](../api/governanceroleassignment-export.md) | octet-stream |Baixe uma coleção de atribuições de função em um recurso e salve como um `.csv` arquivo.|

Não `POST`, `PUT`, `PATCH`ou operações `DELETE` têm suporte no conjunto `roleAssignments` de entidades. Todas as operações de criação, atualização e exclusão são `governanceRoleAssignment` feitas por `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |Cadeia de caracteres     |A ID da atribuição de função. Ele está no formato GUID.|
|resourceId |Cadeia de caracteres     |Obrigatório. A ID do recurso ao qual a atribuição de função está associada. |
|roleDefinitionId|Cadeia de caracteres|Obrigatório. A ID da definição de função à qual a atribuição de função está associada. |
|subjectId|Cadeia de caracteres       |Obrigatório. A ID do assunto ao qual a atribuição de função está associada. |
|linkedEligibleRoleAssignmentId|Cadeia de caracteres|Se este for um e `active assignment` criado devido à ativação em um `eligible assignment`, ele representará a ID disso `eligible assignment`; Caso contrário, o valor será `null`. |
|externalId   |Cadeia de caracteres     |A ID externa do recurso que é usado para identificar a atribuição de função no provedor.|
|startDateTime|DateTimeOffset|A hora de início da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|endDateTime|DateTimeOffset|Para uma atribuição de função não permanente, essa é a hora em que a atribuição de função expirará. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|assignmentState|Cadeia de caracteres  |O estado da atribuição. O valor pode ser `Eligible` para `Active` `Active` atribuição qualificada ou se for atribuído diretamente por administradores ou ativado em uma atribuição qualificada pelos usuários.|
|Membertype|Cadeia de caracteres      |O tipo de membro. O valor pode ser: `Inherited` (se a atribuição de função for herdada de um escopo de recurso pai), `Group` (se a atribuição de função não for herdada, mas vier da associação de uma atribuição de grupo) `User` ou (se a atribuição de função não for herdada nem de uma atribuição de grupo).|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado à atribuição de função. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função associada à atribuição de função. |
|assunto|[governanceSubject](../resources/governancesubject.md)|Somente leitura. O assunto associado à atribuição de função. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Somente leitura. Se este for um e `active assignment` criado devido à ativação em um `eligible assignment`, ele representará o objeto disso `eligible assignment`; Caso contrário, o valor será `null`. |

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


