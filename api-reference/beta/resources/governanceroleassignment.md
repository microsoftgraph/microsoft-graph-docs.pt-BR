---
title: tipo de recurso de governanceRoleAssignment
description: Representa a atribuição de um usuário ou grupo a uma função.
ms.openlocfilehash: 3b0520f4641c961358b2db990914fbdf8de254f8
ms.sourcegitcommit: 82f9d0d10388572a3073b2dde8ca0a7b409135b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2018
ms.locfileid: "27191134"
---
# <a name="governanceroleassignment-resource-type"></a>tipo de recurso de governanceRoleAssignment
> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a atribuição de um usuário ou grupo a uma função.

Gerenciamento de identidade privilegiado (PIM) suporta dois tipos de atribuições:

1. Atribuição ativa - representa o acesso direto/ativado para recursos.
2. Atribuição elegível - representa um estágio intermediário de acesso privilegiado aos recursos, entre nenhum acesso e o acesso direto. Os administradores podem atribuir usuários/grupos para `eligible assignment` com antecedência e sempre que o acesso é necessária, `activation` no `eligible assignment` é necessária para obter o acesso instantâneo ao recurso por várias horas. Após a ativação, um `active assignment` será criado para os membros do grupo de usuários / indicar o status ativado.

## <a name="methods"></a>Métodos

| Método          | Tipo de retorno |Descrição|
|:------------|:--------|:--------|
|[Get](../api/governanceroleassignment-get.md) |  [governanceRoleAssignment](../resources/governanceroleassignment.md) |Leia as propriedades e os relacionamentos de uma entidade de atribuição de função.|
|[List](../api/governanceroleassignment-list.md) | coleção [governanceRoleAssignment](../resources/governanceroleassignment.md)|Uma coleção de atribuições de função em um recurso de lista. |
|[Export](../api/governanceroleassignment-export.md) | fluxo de octeto |Uma coleção de atribuições de função em um recurso de baixar e salvar como um `.csv` arquivo.|

Não `POST`, `PUT`, `PATCH`, ou `DELETE` operações são compatíveis com o `roleAssignments` conjunto de entidade. Qualquer criar, atualizar e excluir operações em `governanceRoleAssignment` são feitas por `governanceRoleAssignmentRequest`.

## <a name="properties"></a>Propriedades
| Propriedade  | Tipo      |Descrição|
|:----------|:----------|:----------|
|id         |String     |A identificação da atribuição de função. Ela está no formato GUID.|
|resourceId |Cadeia de caracteres     |Obrigatório. A identificação do recurso que a atribuição de função é associada. |
|roleDefinitionId|String|Obrigatório. A ID da definição de função que a atribuição de função é associada. |
|subjectId|String       |Obrigatório. A identificação do assunto da qual a atribuição de função é associada. |
|linkedEligibleRoleAssignmentId|String|Caso se trate de um `active assignment` e criados devido a ativação em um `eligible assignment`, que representa a identificação do que `eligible assignment`; Caso contrário, o valor será `null`. |
|externalId   |Cadeia de caracteres     |A identificação do recurso que é usado para identificar a atribuição de função no provedor externa.|
|startDateTime|DateTimeOffset|A hora de início da atribuição de função. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|endDateTime|DateTimeOffset|Para uma atribuição de função de não permanente, esse é o tempo em que a atribuição de função será expirada. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|assignmentState|String  |O estado da atribuição. O valor pode ser <ul><li> `Eligible`para atribuição elegível</li><li> `Active`-se diretamente atribuída `Active` pelos administradores, ou ativado em uma atribuição elegível pelos usuários.</li></ul>|
|memberType|String      |O tipo do membro. O valor pode ser: <ul><li>`Inherited`-a atribuição de função é herdada de um escopo de recurso pai</li><li>`Group`-a atribuição de função não é herdada, mas proveniente a associação de uma atribuição de grupo</li><li>`User`-a atribuição de função é herdada nem nem de atribuição de um grupo.</li></ul>|


## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|recurso|[governanceResource](../resources/governanceresource.md)|Somente leitura. O recurso associado à atribuição de função. |
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Somente leitura. A definição de função associada à atribuição de função. |
|subject|[governanceSubject](../resources/governancesubject.md)|Somente leitura. O assunto associado à atribuição de função. |
|linkedEligibleRoleAssignment|[governanceRoleAssignment](../resources/governanceroleassignment.md)|Somente leitura. Caso se trate de um `active assignment` e criados devido a ativação em um `eligible assignment`, que representa o objeto do que `eligible assignment`; Caso contrário, o valor será `null`. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.


<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
