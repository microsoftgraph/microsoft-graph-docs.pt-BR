---
title: tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote do Access é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 234aad48e11a2b6c5c2a47c494216fa15fbc139b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939212"
---
# <a name="accesspackageassignment-resource-type"></a>tipo de recurso accessPackageAssignment

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure ad pretitulation Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote do Access a um assunto específico, por um período de tempo.  Por exemplo, uma atribuição de pacote de acesso pode indicar que o usuário ' Alice ' tem o acesso atribuído por meio do pacote de acesso ' Sales ' para o período de janeiro de 2019 a julho de 2019.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignments](../api/accesspackageassignment-list.md) | coleção [accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de objetos **accesspackageassignment** . |

>**Observação:** Você não pode usar um método para criar uma atribuição de pacote de acesso. Em vez disso, um cliente que deseja solicitar uma atribuição de pacote de acesso para um usuário pode [criar um accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageId|String|O identificador do pacote de acesso. Somente leitura.|
|assignmentPolicyId|String|O identificador da política de atribuição de pacote do Access. Somente leitura.|
|assignmentstate|String|Somente leitura.|
|assignmentStatus|String|Somente leitura.|
|catalogID|String|O identificador do catálogo que contém o pacote do Access. Somente leitura.|
|expiredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|id|String| Somente leitura.|
|Extended|Booliano|Indica se a atribuição de pacote de acesso é estendida. Somente leitura.|
|targetId|String| A ID do assunto com a atribuição. Somente leitura.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Somente leitura. Anulável.|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Somente leitura. Anulável.|
|accessPackageAssignmentResourceRoles|coleção [accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)| Somente leitura. Anulável.|
|destino|[accessPackageSubject](accesspackagesubject.md)| O assunto da atribuição de pacote do Access. Somente leitura. Anulável.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
            "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
            "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
            "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
            "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
            "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
            "assignmentStatus": "ExpiredNotificationTriggered",
            "assignmentState": "Expired",
            "isExtended": false,
            "expiredDateTime": "2019-04-25T23:45:40.42Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "accessPackageAssignment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
