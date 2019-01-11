---
title: tipo de recurso de privilegedOperationEvent
description: Representa um evento de auditoria que seja gerado pelo gerenciamento de identidades privilegiado para as operações de função, como um administrador gerencia as funções privilegiadas, um usuário ativa sua função e um usuário desativa a sua função.
localization_priority: Normal
ms.openlocfilehash: cc7374f4cf3bc18fbf2f3c36ee4f57e6d703434b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882681"
---
# <a name="privilegedoperationevent-resource-type"></a>tipo de recurso de privilegedOperationEvent

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa um evento de auditoria que seja gerado pelo gerenciamento de identidades privilegiado para as operações de função, como um administrador gerencia as funções privilegiadas, um usuário ativa sua função e um usuário desativa a sua função.


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Lista privilegedOperationEvent](../api/privilegedoperationevent-list.md) | coleção [privilegedOperationEvent](privilegedoperationevent.md) . |Obtenha a coleção de objetos privilegedOperationEvent.|

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|informações adicionais|string|Informações legíveis humanas detalhadas para o evento.|
|creationDateTime|dateTimeOffset|Indica a hora quando o evento for criado.|
|expirationDateTime|dateTimeOffset|Isso é usado apenas quando o requestType é "Ativar" e indica a hora de expiração para a ativação de função.|
|id|string|O identificador exclusivo para privilegedOperationEvent. Somente leitura.|
|referenceKey|string|Número de tíquete de incidente/solicitação durante a ativação de função. O valor é apresentado apenas se o número de tíquete for fornecido durante a ativação de função.|
|referenceSystem|string|Incidente/solicitação fornecido durante a ativação de tole do sistema de registro. O valor é apresentado apenas se o sistema de tíquete é fornecido durante a ativação de função.|
|requestType|string|O tipo de operação de solicitação. O valor de requestType pode ser: ```Assign``` (atribuição de função), ```Activate``` (ativação da função), ```Unassign``` (removem a atribuição de função), ```Deactivate``` (desativação da função), ```ScanAlersNow``` (examinar alertas de segurança), ```DismissAlert``` (descartar o alerta de segurança), ```FixAlertItem``` (corrigir um título alerta problema), ```AccessReview_Review``` (revisar um acesso Revise), ```AccessReview_Create``` (criar um acesso Revise), ```AccessReview_Update``` (atualizar um acesso Revise), e ```AccessReview_Delete``` (excluir um acesso Revise).|
|requestorId|string|A id de usuário do solicitante que inicia a operação.|
|requestorName|string|O nome de usuário do solicitante que inicia a operação.|
|roleId|string|A identificação da função que está associada com a operação.|
|roleName|string|O nome da função.|
|tenantId|string|A id do inquilino (organização).|
|userId|string|A identificação do usuário que está associado com a operação.|
|userMail|string|Email do usuário.|
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
  "userName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "privilegedOperationEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
