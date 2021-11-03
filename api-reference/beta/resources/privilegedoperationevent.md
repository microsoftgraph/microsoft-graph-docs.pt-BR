---
title: Tipo de recurso privilegedOperationEvent
description: Representa um evento de auditoria gerado pelo Privileged Identity Management para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: governance
author: carolinetempleton
ms.openlocfilehash: ddeba79dba2bd3f329d62fff3b90a599f2ceb49a
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60687540"
---
# <a name="privilegedoperationevent-resource-type-deprecated"></a>Tipo de recurso privilegedOperationEvent (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [pim-v1AADRoles-deprecation](../../includes/pim-v1aadroles-deprecation.md)]

Representa um evento de auditoria gerado pelo Privileged Identity Management para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [Coleção privilegedOperationEvent.](privilegedoperationevent.md) |Obter coleção de objetos privilegedOperationEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|cadeia de caracteres|Informações detalhadas de leitura humana para o evento.|
|creationDateTime|DateTimeOffset|Indica a hora em que o evento é criado.|
|expirationDateTime|DateTimeOffset|Isso só é usado quando **o requestType** é , e indica o tempo de expiração `Activate` para a ativação da função.|
|id|cadeia de caracteres|O identificador exclusivo de privilegedOperationEvent. Somente leitura.|
|referenceKey|cadeia de caracteres|Número do tíquete de incidente/solicitação durante a ativação da função. O valor é apresentado somente se o número do tíquete for fornecido durante a ativação da função.|
|referenceSystem|cadeia de caracteres|Sistema de tíquetes de incidente/solicitação fornecido durante a ativação de tole. O valor é apresentado somente se o sistema de tíquetes for fornecido durante a ativação da função.|
|requestType|String|O tipo de operação de solicitação. O valor requestType pode ser: (atribuição de função), (ativação de `Assign` `Activate` `Unassign` função), (remover atribuição de função), `Deactivate` (desativação de função), (verificar alertas de segurança), (descartar alerta de `ScanAlertsNow` segurança), (corrigir um `DismissAlert` `FixAlertItem`  `AccessReview_Review` `AccessReview_Create` `AccessReview_Update` problema de `AccessReview_Delete` alerta de segurança), (revisar uma Revisão do Access), (criar uma Revisão do Access) , (atualizar uma Revisão do Access), (excluir uma Revisão do Access).|
|requestorId|cadeia de caracteres|A ID do usuário do solicitante que inicia a operação.|
|requestorName|cadeia de caracteres|O nome de usuário do solicitante que inicia a operação.|
|roleId|cadeia de caracteres|A id da função associada à operação.|
|roleName|cadeia de caracteres|O nome da função.|
|tenantId|cadeia de caracteres|ID do locatário (organização).|
|userId|cadeia de caracteres|A id do usuário associado à operação.|
|userMail|cadeia de caracteres|O email do usuário.|
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


