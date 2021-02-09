---
title: Tipo de recurso directRoutingLogRow
description: Representa uma linha de dados no log de chamadas de roteamento direto.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 21104f3d0812edd2af7918d6b55ff9a2f9013037
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159651"
---
# <a name="directroutinglogrow-resource-type"></a>Tipo de recurso directRoutingLogRow

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha de dados no log de chamadas de roteamento direto. Cada linha mapeia para uma chamada.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da chamada. GUID.|
|correlationId|Cadeia de caracteres|Identificador da chamada que você pode usar ao chamar o Suporte da Microsoft. GUID.|
|userId|Cadeia de caracteres|Chamar a ID do usuário no Graph. Essa e outras informações do usuário serão nulas/vazias para tipos de chamada de bot. GUID.|
|userPrincipalName|String|UserPrincipalName (nome de login) no Azure Active Directory. Isso geralmente é o mesmo endereço SIP do usuário e pode ser igual ao endereço de email do usuário.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário.|
|startDateTime|DateTimeOffset|Hora do início da chamada.<br/>Para chamadas com falha e não respondidas, isso pode ser igual ao tempo de convite ou falha.|
|inviteDateTime|DateTimeOffset| Quando o convite inicial foi enviado.|
|failureDateTime|DateTimeOffset| Existe apenas para chamadas com falha (não totalmente estabelecidas).|
|endDateTime|DateTimeOffset| Existe apenas para chamadas bem-sucedidas (totalmente estabelecidas). Hora em que a chamada terminou.|
|duração|Int32| Duração da chamada em segundos.|
|callType|String| Tipo e direção da chamada.|
|successfulCall|Boolean| Sucesso ou tentativa.|
|callerNumber|String| Número do usuário ou bot que fez a chamada. [Formato E.164,](https://en.wikipedia.org/wiki/E.164) mas pode incluir dados adicionais.|
|calleeNumber|String| Número do usuário ou bot que recebeu a chamada. [Formato E.164,](https://en.wikipedia.org/wiki/E.164) mas pode incluir dados adicionais.|
|mediaPathLocation|String| O datacenter usado para o caminho de mídia em uma chamada sem desvio.|
|signalingLocation|String| O datacenter usado para sinalização para chamadas de bypass e não bypass.|
|finalSipCode|Int32| O código com o qual a chamada terminou, [RFC 3261](https://tools.ietf.org/html/rfc3261).|
|callEndSubReason|Int32| Além dos códigos SIP, a Microsoft possui subcódigos próprios que indicam o problema específico.|
|finalSipCodePhrase|String| Descrição do código SIP e do subcódigo da Microsoft.|
|trunkFullyQualifiedDomainName|String| Nome de domínio totalmente qualificado do controlador de borda da sessão.|
|mediaBypassEnabled|Boolean| Indica se o tronco foi habilitado para bypass de mídia ou não.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.directRoutingLogRow",
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


