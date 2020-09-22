---
title: tipo de recurso privilegedOperationEvent
description: Representa um evento de auditoria que é gerado pelo gerenciamento de identidade privilegiado para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 02da3f408506560ba91f8139bb7bf64d0ca749dd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070531"
---
# <a name="privilegedoperationevent-resource-type"></a>tipo de recurso privilegedOperationEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um evento de auditoria que é gerado pelo gerenciamento de identidade privilegiado para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List privilegedOperationEvent](../api/privilegedoperationevent-list.md) | coleção [privilegedOperationEvent](privilegedoperationevent.md) . |Obtém a coleção de objetos privilegedOperationEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|cadeia de caracteres|Informações detalhadas sobre a leitura humana para o evento.|
|creationDatetime|dateTimeOffset|Indica a hora em que o evento é criado.|
|expirationDateTime|dateTimeOffset|Isso é usado apenas quando RequestType é "Activate" e indica o tempo de expiração da ativação da função.|
|id|cadeia de caracteres|O identificador exclusivo para o privilegedOperationEvent. Somente leitura.|
|referenceKey|cadeia de caracteres|Número do tíquete de solicitação/incidente durante a ativação de função. O valor é apresentado somente se o número do tíquete for fornecido durante a ativação de função.|
|referenceSystem|cadeia de caracteres|Sistema de tíquetes de solicitações/incidentes fornecido durante a ativação do Tole. O valor é apresentado somente se o sistema de tíquete for fornecido durante a ativação de função.|
|RequestType|cadeia de caracteres|O tipo de operação de solicitação. O valor de RequestType pode ser: ```Assign``` (atribuição de função), ```Activate``` (ativação de função), ```Unassign``` (atribuição de função remover), ( ```Deactivate``` desativação de função), (examinar alertas de segurança), (ignorar o alerta de segurança), (corrigir um problema de alerta de segurança), ( ```ScanAlersNow``` ```DismissAlert``` ```FixAlertItem``` ```AccessReview_Review``` revisar uma ```AccessReview_Create``` ```AccessReview_Update``` ```AccessReview_Delete``` revisão de acesso)|
|requestorId|cadeia de caracteres|A ID de usuário do solicitante que inicia a operação.|
|requestorName|cadeia de caracteres|O nome de usuário do solicitante que inicia a operação.|
|roleId|cadeia de caracteres|A ID da função associada à operação.|
|roleName|cadeia de caracteres|O nome da função.|
|tenantId|cadeia de caracteres|A ID do locatário (organização).|
|userId|cadeia de caracteres|A ID do usuário associada à operação.|
|usermail|cadeia de caracteres|O email do usuário.|
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


