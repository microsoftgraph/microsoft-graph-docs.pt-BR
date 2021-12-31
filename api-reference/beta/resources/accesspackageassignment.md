---
title: Tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: b394efdd7ac2cbc97ff1245af4e0d01d4392e3f4
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650619"
---
# <a name="accesspackageassignment-resource-type"></a>Tipo de recurso accessPackageAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-overview.md), uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.  Por exemplo, uma atribuição de pacote de acesso pode dizer que a usuária Alice recebeu acesso por meio do pacote de acesso Vendas do período de janeiro de 2019 a julho de 2019.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md) | [Coleção accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de **objetos accessPackageAssignment.** |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário de entrada.|
| [reprocessamento](../api/accesspackageassignment-reprocess.md) | Nenhum | Reavaliar automaticamente e impor as atribuições de um usuário para um pacote de acesso específico.|

> [!NOTE]
> Para criar ou remover uma atribuição de pacote de acesso para um usuário, use [a criação de um accessPackageAssignmentRequest](../api/entitlementmanagement-post-accesspackageassignmentrequests.md)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageId|String|O identificador do pacote de acesso. Somente leitura.|
|assignmentPolicyId|String|O identificador da política de atribuição do pacote de acesso. Somente leitura.|
|assignmentState|String|O estado da atribuição do pacote de acesso. Os valores possíveis `Delivering` são `Delivered` , ou `Expired` . Somente leitura. Suporta `$filter` (`eq`).|
|assignmentStatus|String|Mais informações sobre o ciclo de vida da atribuição.  Os valores possíveis `Delivering` `Delivered` incluem , `NearExpiry1DayNotificationTriggered` , ou `ExpiredNotificationTriggered` .  Somente leitura.|
|catalogId|String|O identificador do catálogo que contém o pacote de acesso. Somente leitura.|
|expiredDateTime|DateTimeOffset|O tipo de carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1º de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|String| Somente leitura.|
|isExtended|Booliano|Indica se a atribuição do pacote de acesso foi estendida. Somente leitura.|
|targetId|String| A ID do assunto com a atribuição. Somente leitura.|
|Cronograma|[requestSchedule](requestschedule.md)| Quando a atribuição de acesso estiver no local. Somente leitura.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Somente leitura. Anulável. Suporta `$filter` ( ) na propriedade `eq` **id** `$expand` e parâmetros de consulta.|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Somente leitura. Anulável. Suporta `$filter` ( ) na propriedade `eq` **id**|
|accessPackageAssignmentResourceRoles|[Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)| As funções de recurso entregues ao usuário de destino para essa atribuição. Somente leitura. Anulável.|
|destino|[accessPackageSubject](accesspackagesubject.md)| O assunto da atribuição do pacote de acesso. Somente leitura. Anulável. Suporta o `$expand`. Suporta `$filter` ( ) em `eq` **objectId**. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "keyProperty": "id"
}-->

```json
{
   "id":"9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
   "catalogId":"cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
   "accessPackageId":"e3f47362-993f-4fcb-8a38-532ffca16150",
   "assignmentPolicyId":"63ebd106-8116-40e7-a0ab-01ae475d11bb",
   "targetId":"ab4291f6-66b7-42bf-b597-a05b29414f5c",
   "assignmentStatus":"ExpiredNotificationTriggered",
   "assignmentState":"Expired",
   "isExtended":false,
   "expiredDateTime":"2019-04-25T23:45:40.42Z"
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
