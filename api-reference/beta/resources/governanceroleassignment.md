---
title: Tipo de recurso governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7206bea058910aa24d6dd907ea495acb6cace0aa
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443101"
---
# <a name="governanceroleassignment-resource-type"></a>Tipo de recurso governanceRoleAssignment

Namespace: microsoft.graph [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa a atribuição de um usuário ou grupo a uma função.

O PIM (Privileged Identity Management) dá suporte a dois tipos de atribuições:

1. Atribuição ativa - Representa o acesso direto/ativado aos recursos.
2. Atribuição qualificada - representa um estágio intermediário de acesso privilegiado a recursos, entre nenhum acesso e acesso direto. Os administradores podem atribuir usuários/grupos com antecedência e, sempre que o acesso for necessário, o acesso é necessário para obter o acesso instantâneo ao recurso `eligible assignment` `activation` por várias `eligible assignment` horas. Após a ativação, `active assignment` um será criado para os usuários/membros do grupo indicarem o status ativado.

## <a name="methods"></a>Methods

| Método          | Tipo de retorno |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Ler propriedades e relações de uma entidade de atribuição de função.|
|[List](../api/governanceroleassignment-list.md) | [Coleção governanceRoleAssignment](../resources/governanceroleassignment.md)|Listar uma coleção de atribuições de função em um recurso. |
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
|startDateTime|DateTimeOffset|A hora de início da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Para uma atribuição de função não permanente, este é o momento em que a atribuição de função será expirada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|assignmentState|String  |O estado da atribuição. O valor pode ser <ul><li> `Eligible` para atribuição qualificada</li><li> `Active` - se ele for atribuído diretamente pelos administradores ou ativado em uma `Active` atribuição qualificada pelos usuários.</li></ul>|
|memberType|String      |O tipo de membro. O valor pode ser: <ul><li>`Inherited` - a atribuição de função é herdada de um escopo de recurso pai</li><li>`Group`- a atribuição de função não é herdada, mas vem da associação de uma atribuição de grupo</li><li>`User` - a atribuição de função não é herdada nem de uma atribuição de grupo.</li></ul>|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado à atribuição de função. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função associada à atribuição de função. |
|assunto|[governanceSubject](../resources/governancesubject.md)|Somente leitura. O assunto associado à atribuição de função. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Somente leitura. Se for um `active assignment` e criado devido à ativação em um , ele `eligible assignment` representará o objeto disso `eligible assignment` ; Caso contrário, o valor será `null` . |

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


