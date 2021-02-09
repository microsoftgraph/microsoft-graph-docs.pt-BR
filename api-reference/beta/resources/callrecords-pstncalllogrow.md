---
title: Tipo de recurso pstnCallLogRow
description: Representa uma linha de dados no log de chamadas da PSTN (Rede Telefônica Pública comu pt-br).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5103404bdaa6ac4eafbfcffd45deef41c217600a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155577"
---
# <a name="pstncalllogrow-resource-type"></a>Tipo de recurso pstnCallLogRow

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha de dados no log de chamadas da PSTN (Rede Telefônica Pública comu pt-br). Cada linha mapeia para uma chamada.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da chamada. GUID.|
|callId|String|Identificador de chamada. Não há garantia de ser exclusivo.|
|userId|Cadeia de caracteres|Chamar a ID do usuário no Graph. GUID. Essa e outras informações do usuário serão nulas/vazias para tipos de chamada de bot (ucap_in, ucap_out).|
|userPrincipalName|String|UserPrincipalName (nome de login) no Azure Active Directory. Isso geralmente é o mesmo endereço SIP do usuário e pode ser igual ao endereço de email do usuário.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário.|
|startDateTime|DateTimeOffset|Hora do início da chamada.|
|endDateTime|DateTimeOffset|Hora da finalização da chamada.|
|duração|Int32|Quanto tempo a chamada foi conectada, em segundos.|
|charge|Duplo|Valor em dinheiro ou custo da chamada que é cobrada em sua conta.|
|callType|String|Se a chamada foi uma chamada de saída ou de entrada PSTN e o tipo de chamada, como uma chamada feita por um usuário ou uma conferência de áudio.|
|currency|String|Tipo de moeda usado para calcular o custo da chamada ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).|
|calleeNumber|String|Número discado no [formato E.164.](https://en.wikipedia.org/wiki/E.164)|
|usageCountryCode|String|Código do país do usuário, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|tenantCountryCode|String|Código do país do locatário, [ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|connectionCharge|Duplo|Preço da taxa de conexão.|
|callerNumber|String|Número que recebeu a chamada para chamadas de entrada ou o número discado para chamadas de saída. Formato E.164.|
|destinationContext|String|Se a chamada foi doméstica (dentro de um país ou região) ou internacional (fora de um país ou região) com base na localização do usuário.|
|destinationName|String|País ou região discada.|
|conferenceId|String|ID da audioconferência.|
|licenseCapability|String|A licença usada para a chamada.|
|inventoryType|String|Tipo de número de telefone do usuário, como um serviço de número gratuito.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "keyProperty": "id"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.callRecords.pstnCallLogRow",
  "id": "String (identifier)",
  "callId": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "duration": "Integer",
  "charge": "Double",
  "callType": "String",
  "currency": "String",
  "calleeNumber": "String",
  "usageCountryCode": "String",
  "tenantCountryCode": "String",
  "connectionCharge": "Double",
  "callerNumber": "String",
  "destinationContext": "String",
  "destinationName": "String",
  "conferenceId": "String",
  "licenseCapability": "String",
  "inventoryType": "String"
}
```


