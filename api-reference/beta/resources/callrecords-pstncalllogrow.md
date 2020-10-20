---
title: tipo de recurso pstnCallLogRow
description: Representa uma linha de dados no log de chamadas de rede telefônica de comutador público (PSTN).
author: williamlooney
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bc83f3304eeb918d665b2651fda9809fd8a05880
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601668"
---
# <a name="pstncalllogrow-resource-type"></a>tipo de recurso pstnCallLogRow

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha de dados no log de chamadas de rede telefônica de comutador público (PSTN). Cada linha é mapeada para uma chamada.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de chamada exclusivo. #C0.|
|callId|String|Identificador de chamada. Não é garantido como exclusivo.|
|userId|Cadeia de caracteres|Chamar a ID do usuário no Graph. #C0. Esta e outras informações do usuário serão nulas/vazias para tipos de chamada de bot (ucap_in ucap_out).|
|userPrincipalName|String|UserPrincipalName (nome de entrada) no Azure Active Directory. Isso geralmente é o mesmo que o endereço SIP do usuário e pode ser o mesmo que o endereço de email do usuário.|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário.|
|startDateTime|DateTimeOffset|Hora do início da chamada.|
|endDateTime|DateTimeOffset|Hora da finalização da chamada.|
|duração|Int32|Quanto tempo a chamada foi conectada, em segundos.|
|adicional|Duplo|Quantidade de dinheiro ou custo da chamada cobrada em sua conta.|
|callType|String|Se a chamada foi uma chamada PSTN de saída ou de entrada e o tipo de chamada, como uma chamada feita por um usuário ou uma conferência de áudio.|
|moeda|String|Tipo de moeda usada para calcular o custo da chamada ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).|
|calleeNumber|String|Número discado no formato [E. 164](https://en.wikipedia.org/wiki/E.164) .|
|usageCountryCode|String|Código do país do usuário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|tenantCountryCode|String|Código do país do locatário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|connectionCharge|Duplo|Preço da taxa de conexão.|
|callerNumber|String|Número que recebeu a chamada para chamadas de entrada ou o número discado para chamadas de saída. Formato E. 164.|
|destinationContext|String|Se a chamada foi doméstica (dentro de um país ou região) ou internacional (fora de um país ou região) com base no local do usuário.|
|destinationname|String|País ou região discada.|
|ID|String|ID da conferência de áudio.|
|licenseCapability|String|A licença usada para a chamada.|
|inventorytype|String|Tipo de número de telefone do usuário, como um serviço de número de chamada gratuita.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "ignored",
  "@odata.type": "microsoft.graph.callRecords.pstnCallLogRow",
  "baseType": "",
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


