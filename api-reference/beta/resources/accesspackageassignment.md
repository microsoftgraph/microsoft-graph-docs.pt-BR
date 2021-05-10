---
title: Tipo de recurso accessPackageAssignment
description: Uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: fd352fe67c3afabb1819ffc58d7081dbdae1525c
ms.sourcegitcommit: c5cc948c764b4daab861aadb390b827f658a9b7f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2021
ms.locfileid: "52298509"
---
# <a name="accesspackageassignment-resource-type"></a>Tipo de recurso accessPackageAssignment

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

No [Azure AD Entitlement Management](entitlementmanagement-root.md), uma atribuição de pacote de acesso é uma atribuição de um pacote de acesso a um assunto específico, por um período de tempo.  Por exemplo, uma atribuição de pacote de acesso pode dizer que a usuária Alice recebeu acesso por meio do pacote de acesso Vendas do período de janeiro de 2019 a julho de 2019.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [Listar accessPackageAssignments](../api/accesspackageassignment-list.md) | [Coleção accessPackageAssignment](accesspackageassignment.md) | Recupere uma lista de **objetos accessPackageAssignment.** |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[Coleção accessPackageAssignment](../resources/accesspackageassignment.md)|Recupere a lista de **objetos accessPackageAssignment** filtrados no usuário de entrada.|

>**Observação:** Não é possível usar um método para criar ou remover uma atribuição de pacote de acesso. Em vez disso, um cliente que deseja solicitar uma atribuição de pacote de acesso para um usuário ou remover uma atribuição de pacote de acesso de um usuário pode criar um [accessPackageAssignmentRequest](../api/accesspackageassignmentrequest-post.md).

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackageId|Cadeia de caracteres|O identificador do pacote de acesso. Somente leitura.|
|assignmentPolicyId|Cadeia de caracteres|O identificador da política de atribuição do pacote de acesso. Somente leitura.|
|assignmentState|Cadeia de caracteres|O estado da atribuição do pacote de acesso. Os valores possíveis `Delivering` são `Delivered` , ou `Expired` . Somente leitura.|
|assignmentStatus|Cadeia de caracteres|Mais informações sobre o ciclo de vida da atribuição.  Os valores possíveis `Delivering` `Delivered` incluem , `NearExpiry1DayNotificationTriggered` , ou `ExpiredNotificationTriggered` .  Somente leitura.|
|catalogId|Cadeia de caracteres|O identificador do catálogo que contém o pacote de acesso. Somente leitura.|
|expiredDateTime|DateTimeOffset|O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`|
|id|String| Somente leitura.|
|isExtended|Booliano|Indica se a atribuição do pacote de acesso foi estendida. Somente leitura.|
|targetId|Cadeia de caracteres| A ID do assunto com a atribuição. Somente leitura.|
|Cronograma|[requestSchedule](requestschedule.md)| Quando a atribuição de acesso estiver no local. Somente leitura.|

## <a name="relationships"></a>Relações

| Relação | Tipo        | Descrição |
|:-------------|:------------|:------------|
|accessPackage|[accessPackage](accesspackage.md)| Somente leitura. Anulável.|
|accessPackageAssignmentPolicy|[accessPackageAssignmentPolicy](accesspackageassignmentpolicy.md)| Somente leitura. Anulável.|
|accessPackageAssignmentResourceRoles|[Coleção accessPackageAssignmentResourceRole](accesspackageassignmentresourcerole.md)| As funções de recurso entregues ao usuário de destino para essa atribuição. Somente leitura. Anulável.|
|destino|[accessPackageSubject](accesspackagesubject.md)| O assunto da atribuição do pacote de acesso. Somente leitura. Anulável.|

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


