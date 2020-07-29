---
title: tipo de recurso directRoutingLogRow
description: Representa uma linha de dados no log de chamadas de roteamento direto.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3a01ed8410532264fceb0164ef4f703b636ccdef
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510037"
---
# <a name="directroutinglogrow-resource-type"></a>tipo de recurso directRoutingLogRow

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha de dados no log de chamadas de roteamento direto. Cada linha é mapeada para uma chamada.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de chamada exclusivo. #C0.|
|correlationId|Cadeia de caracteres|Identificador para a chamada que você pode usar ao chamar o suporte da Microsoft. #C0.|
|userId|Cadeia de caracteres|Chamar a ID do usuário no Graph. Esta e outras informações do usuário serão nulas/vazias para tipos de chamada de bot. #C0.|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName (nome de entrada) no Azure Active Directory. Isso geralmente é o mesmo que o endereço SIP do usuário e pode ser o mesmo que o endereço de email do usuário.|
|userDisplayName|String|Nome de exibição do usuário.|
|startDateTime|DateTimeOffset|Hora do início da chamada.<br/>Para chamadas com falha e não atendidas, isso pode ser igual ao tempo de convite ou de falha.|
|inviteDateTime|DateTimeOffset| Quando o convite inicial foi enviado.|
|failureDateTime|DateTimeOffset| Existe somente para chamadas com falha (não totalmente estabelecidas).|
|endDateTime|DateTimeOffset| Existe somente para chamadas bem-sucedidas (totalmente estabelecidas). Hora em que a chamada terminou.|
|duration|Int32| Duração da chamada em segundos.|
|callType|Cadeia de caracteres| Tipo de chamada e direção.|
|successfulCall|Boolean| Êxito ou tentativa.|
|callerNumber|Cadeia de caracteres| Número do usuário ou do bot que fez a chamada. Formato [e. 164](https://en.wikipedia.org/wiki/E.164) , mas pode incluir dados adicionais.|
|calleeNumber|Cadeia de caracteres| Número do usuário ou do bot que recebeu a chamada. Formato [e. 164](https://en.wikipedia.org/wiki/E.164) , mas pode incluir dados adicionais.|
|mediaPathLocation|Cadeia de caracteres| O datacenter usado para o caminho de mídia em chamada não bypass.|
|signalingLocation|Cadeia de caracteres| O datacenter usado para sinalização para as chamadas bypass e non-bypass.|
|finalSipCode|Int32| O código com o qual a chamada terminou, [RFC 3261](https://tools.ietf.org/html/rfc3261).|
|callEndSubReason|Int32| Além dos códigos SIP, a Microsoft possui subcódigos que indicam o problema específico.|
|finalSipCodePhrase|Cadeia de caracteres| Descrição do código SIP e do subcódigo da Microsoft.|
|trunkFullyQualifiedDomainName|Cadeia de caracteres| Nome de domínio totalmente qualificado do controlador de borda da sessão.|
|mediaBypassEnabled|Boolean| Indica se o tronco foi habilitado para bypass de mídia ou não.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
  "baseType": "",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.directRoutingLogRow",
  "id": "String (identifier)",
  "correlationId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "inviteDateTime": "String (timestamp)",
  "failureDateTime": "String (timestamp)",
  "duration": "Integer",
  "callType": "String",
  "successfulCall": "Boolean",
  "callerNumber": "String",
  "calleeNumber": "String",
  "mediaPathLocation": "String",
  "signalingLocation": "String",
  "finalSipCode": "Integer",
  "callEndSubReason": "Integer",
  "finalSipCodePhrase": "String",
  "trunkFullyQualifiedDomainName": "String",
  "mediaBypassEnabled": "Boolean"
}
```
