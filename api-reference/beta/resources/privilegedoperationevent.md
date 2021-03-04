---
title: Tipo de recurso privilegedOperationEvent
description: Representa um evento de auditoria gerado pelo Privileged Identity Management para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 408eb2ca06168b4e22b945aa9d3d6faa2b1a561a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440140"
---
# <a name="privilegedoperationevent-resource-type"></a>Tipo de recurso privilegedOperationEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um evento de auditoria gerado pelo Privileged Identity Management para as operações de função, como um administrador gerencia funções privilegiadas, um usuário ativa sua função e um usuário desativa sua função.


## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[List privilegedOperationEvent](../api/privilegedoperationevent-list.md) | [Coleção privilegedOperationEvent.](privilegedoperationevent.md) |Obter coleção de objetos privilegedOperationEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|string|Informações detalhadas de leitura humana para o evento.|
|creationDateTime|dateTimeOffset|Indica a hora em que o evento é criado.|
|expirationDateTime|dateTimeOffset|Isso só é usado quando o requestType é "Activate", e indica o tempo de expiração para a ativação da função.|
|id|string|O identificador exclusivo de privilegedOperationEvent. Somente leitura.|
|referenceKey|string|Número do tíquete de incidente/solicitação durante a ativação da função. O valor é apresentado somente se o número do tíquete for fornecido durante a ativação da função.|
|referenceSystem|string|Sistema de tíquetes de incidente/solicitação fornecido durante a ativação de tole. O valor é apresentado somente se o sistema de tíquetes for fornecido durante a ativação da função.|
|requestType|string|O tipo de operação de solicitação. O valor requestType pode ser: (atribuição de função), (ativação de ```Assign``` ```Activate``` função), ```Unassign``` (remover atribuição de função), ```Deactivate``` (desativação de função), (verificar alertas de segurança), (descartar alerta de ```ScanAlersNow``` segurança), (corrigir um ```DismissAlert``` ```FixAlertItem``` ```AccessReview_Review``` ```AccessReview_Create``` ```AccessReview_Update``` problema de ```AccessReview_Delete``` alerta de segurança), (revisar uma Revisão do Access), (criar uma Revisão do Access), (atualizar uma Revisão do Access) e (excluir uma Revisão do Access).|
|requestorId|string|A ID do usuário do solicitante que inicia a operação.|
|requestorName|string|O nome de usuário do solicitante que inicia a operação.|
|roleId|string|A id da função associada à operação.|
|roleName|string|O nome da função.|
|tenantId|cadeia de caracteres|ID do locatário (organização).|
|userId|cadeia de caracteres|A id do usuário associado à operação.|
|userMail|string|O email do usuário.|
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


