---
title: Tipo de recurso privilegedOperationEvent
description: Representa um evento de auditoria gerado pelo Privileged Identity Management para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: rkarim-ms
ms.openlocfilehash: 0002e10cff2324d60f9000b1cdf961b865409056
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65397534"
---
# <a name="privilegedoperationevent-resource-type-deprecated"></a>Tipo de recurso privilegedOperationEvent (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v2AADRoles-deprecation](../../includes/pim-v2AADRoles-deprecation.md)]

Representa um evento de auditoria gerado pelo Privileged Identity Management para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [Coleção privilegedOperationEvent](privilegedoperationevent.md) . |Obter coleção de objetos privilegedOperationEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|string|Informações detalhadas legíveis para o evento.|
|creationDateTime|DateTimeOffset|Indica a hora em que o evento é criado.|
|expirationDateTime|DateTimeOffset|Isso só é usado quando **o requestType** é `Activate`, e indica o tempo de expiração para a ativação da função.|
|id|string|O identificador exclusivo de privilegedOperationEvent. Somente leitura.|
|referenceKey|cadeia de caracteres|Número do tíquete de solicitação/incidente durante a ativação da função. O valor será apresentado somente se o número do tíquete for fornecido durante a ativação da função.|
|referenceSystem|cadeia de caracteres|Sistema de tíquetes de incidente/solicitação fornecido durante a ativação de tole. O valor será apresentado somente se o sistema de tíquetes for fornecido durante a ativação da função.|
|Requesttype|Cadeia de caracteres|O tipo de operação de solicitação. O valor requestType pode ser: `Assign` (atribuição de função), `Activate` (ativação de função), `Unassign` (remover atribuição de função), `Deactivate` (desativação de função), `ScanAlertsNow` (examinar alertas de segurança), `DismissAlert` (ignorar alerta de segurança), `FixAlertItem` (corrigir um problema de alerta de segurança),  `AccessReview_Review` (examinar uma Revisão de Acesso), `AccessReview_Create` (criar uma Revisão de Acesso), `AccessReview_Update` (atualizar uma Revisão de Acesso) `AccessReview_Delete` (excluir uma Revisão de Acesso).|
|requestorId|string|A ID de usuário do solicitante que inicia a operação.|
|requestorName|cadeia de caracteres|O nome de usuário do solicitante que inicia a operação.|
|roleId|string|A ID da função associada à operação.|
|Rolename|cadeia de caracteres|O nome da função.|
|tenantId|cadeia de caracteres|A ID do locatário (organização).|
|userId|cadeia de caracteres|A ID do usuário que está associado à operação.|
|userMail|string|O email do usuário.|
|userName|cadeia de caracteres|O nome de exibição do usuário.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedOperationEvent"
}-->

```json
{
  "additionalInformation": "string",
  "creationDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "requestType": "string",
  "requestorId": "string",
  "requestorName": "string",
  "roleId": "string",
  "roleName": "string",
  "tenantId": "string",
  "userId": "string",
  "userMail": "string",
  "userName": "string",
  "referenceKey": "string",
  "referenceSystem": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


