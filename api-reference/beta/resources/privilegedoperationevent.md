---
title: tipo de recurso privilegedOperationEvent
description: Representa um evento de auditoria que é gerado pelo gerenciamento de identidade privilegiado para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 921fa2068d152652b41f36b8893859df7696b5a8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521520"
---
# <a name="privilegedoperationevent-resource-type"></a>tipo de recurso privilegedOperationEvent

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um evento de auditoria que é gerado pelo gerenciamento de identidade privilegiado para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List privilegedOperationEvent](../api/privilegedoperationevent-list.md) | coleção [privilegedOperationEvent](privilegedoperationevent.md) . |Obtém a coleção de objetos privilegedOperationEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|string|Informações detalhadas sobre a leitura humana para o evento.|
|creationDatetime|dateTimeOffset|Indica a hora em que o evento é criado.|
|expirationDateTime|dateTimeOffset|Isso é usado apenas quando RequestType é "Activate" e indica o tempo de expiração da ativação da função.|
|id|string|O identificador exclusivo para o privilegedOperationEvent. Somente leitura.|
|referenceKey|string|Número do tíquete de solicitação/incidente durante a ativação de função. O valor é apresentado somente se o número do tíquete for fornecido durante a ativação de função.|
|referenceSystem|string|Sistema de tíquetes de solicitações/incidentes fornecido durante a ativação do Tole. O valor é apresentado somente se o sistema de tíquete for fornecido durante a ativação de função.|
|RequestType|string|O tipo de operação de solicitação. O valor de RequestType pode ```Assign``` ser: (atribuição de ```Activate``` função), (ativação ```Unassign``` de função), (atribuição ```Deactivate``` de função remover), ( ```ScanAlersNow``` desativação de função) ```DismissAlert``` , (examinar alertas de segurança ```FixAlertItem``` ), (ignorar o alerta de segurança ```AccessReview_Review``` ), (corrigir um problema de ```AccessReview_Create``` alerta de segurança), (revisar uma ```AccessReview_Update``` ```AccessReview_Delete``` revisão de acesso)|
|requestorId|string|A ID de usuário do solicitante que inicia a operação.|
|requestorName|string|O nome de usuário do solicitante que inicia a operação.|
|roleId|string|A ID da função associada à operação.|
|roleName|string|O nome da função.|
|tenantId|cadeia de caracteres|A ID do locatário (organização).|
|userId|string|A ID do usuário associada à operação.|
|usermail|string|O email do usuário.|
|userName|string|O nome de exibição do usuário.|

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
