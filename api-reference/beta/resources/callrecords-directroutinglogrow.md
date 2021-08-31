---
title: Tipo de recurso directRoutingLogRow
description: Representa uma linha de dados no log de chamadas de roteamento direto.
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a1260d3f1406807930e696a1d7adbd6db21392b6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788244"
---
# <a name="directroutinglogrow-resource-type"></a>Tipo de recurso directRoutingLogRow

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha de dados no log de chamadas de roteamento direto. Cada linha mapeia para uma chamada.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [getDirectRoutingCalls](../api/callrecords-callrecord-getdirectroutingcalls.md) | [coleção microsoft.graph.callRecords.directRoutingLogRow](callrecords-directroutinglogrow.md)| Listar **objetos directRoutingLogRow** para um registro de chamada. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callEndSubReason|Int32| Além dos códigos SIP, a Microsoft tem subcódigos próprios que indicam o problema específico.|
|callType|Cadeia de caracteres| Tipo e direção de chamada.|
|calleeNumber|Cadeia de caracteres| Número do usuário ou bot que recebeu a chamada. [Formato E.164,](https://en.wikipedia.org/wiki/E.164) mas pode incluir dados adicionais.|
|callerNumber|Cadeia de caracteres| Número do usuário ou bot que fez a chamada. [Formato E.164,](https://en.wikipedia.org/wiki/E.164) mas pode incluir dados adicionais.|
|correlationId|Cadeia de caracteres|Identificador da chamada que você pode usar ao chamar o Suporte da Microsoft. GUID.|
|duração|Int32| Duração da chamada em segundos.|
|endDateTime|DateTimeOffset| Só existe para chamadas bem-sucedidas (totalmente estabelecidas). Hora em que a chamada terminou.|
|failureDateTime|DateTimeOffset| Só existe para chamadas com falha (não totalmente estabelecidas).|
|finalSipCodePhrase|Cadeia de caracteres| Descrição do código SIP e subcódigo da Microsoft.|
|finalSipCode|Int32| O código com o qual a chamada terminou, [RFC 3261](https://tools.ietf.org/html/rfc3261).|
|id|Cadeia de caracteres|Identificador de chamada exclusivo. GUID.|
|inviteDateTime|DateTimeOffset| Quando o convite inicial foi enviado.|
|mediaBypassEnabled|Boleano| Indica se o tronco foi habilitado para bypass de mídia ou não.|
|mediaPathLocation|Cadeia de caracteres| O datacenter usado para o caminho de mídia em chamada não ignorada.|
|signalingLocation|Cadeia de caracteres| O datacenter usado para sinalização para chamadas de bypass e não bypass.|
|startDateTime|DateTimeOffset|Hora do início da chamada.<br/>Para chamadas com falha e sem resposta, isso pode ser igual a tempo de convite ou falha.|
|successfulCall|Boleano| Sucesso ou tentativa.|
|trunkFullyQualifiedDomainName|Cadeia de caracteres| Nome de domínio totalmente qualificado do controlador de borda de sessão.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário.|
|userId|Cadeia de caracteres|Chamando a ID do usuário Graph. Essa e outras informações de usuário serão nulas/vazias para tipos de chamada de bot. GUID.|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName (nome de login) no Azure Active Directory. Isso geralmente é o mesmo que o Endereço SIP do usuário e pode ser igual ao endereço de email do usuário.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
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
  "endDateTime": "String (timestamp)",
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


