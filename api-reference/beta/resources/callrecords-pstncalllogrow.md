---
title: tipo de recurso pstnCallLogRow
description: Representa uma linha de dados no log de chamadas de rede telefônica de comutador público (PSTN).
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: fdcaaa311ea3d1f875bd3933420cfed058ef7808
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509966"
---
# <a name="pstncalllogrow-resource-type"></a>tipo de recurso pstnCallLogRow

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma linha de dados no log de chamadas de rede telefônica de comutador público (PSTN). Cada linha é mapeada para uma chamada.

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador de chamada exclusivo. #C0.|
|callId|Cadeia de caracteres|Identificador de chamada. Não é garantido como exclusivo.|
|userId|Cadeia de caracteres|Chamar a ID do usuário no Graph. #C0. Esta e outras informações do usuário serão nulas/vazias para tipos de chamada de bot (ucap_in ucap_out).|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName (nome de entrada) no Azure Active Directory. Isso geralmente é o mesmo que o endereço SIP do usuário e pode ser o mesmo que o endereço de email do usuário.|
|userDisplayName|String|Nome de exibição do usuário.|
|startDateTime|DateTimeOffset|Hora do início da chamada.|
|endDateTime|DateTimeOffset|Hora da finalização da chamada.|
|duration|Int32|Quanto tempo a chamada foi conectada, em segundos.|
|adicional|Duplo|Quantidade de dinheiro ou custo da chamada cobrada em sua conta.|
|callType|Cadeia de caracteres|Se a chamada foi uma chamada PSTN de saída ou de entrada e o tipo de chamada, como uma chamada feita por um usuário ou uma conferência de áudio.|
|moeda|Cadeia de caracteres|Tipo de moeda usada para calcular o custo da chamada ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).|
|calleeNumber|Cadeia de caracteres|Número discado no formato [E. 164](https://en.wikipedia.org/wiki/E.164) .|
|usageCountryCode|Cadeia de caracteres|Código do país do usuário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|tenantCountryCode|Cadeia de caracteres|Código do país do locatário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|connectionCharge|Duplo|Preço da taxa de conexão.|
|callerNumber|Cadeia de caracteres|Número que recebeu a chamada para chamadas de entrada ou o número discado para chamadas de saída. Formato E. 164.|
|destinationContext|Cadeia de caracteres|Se a chamada foi doméstica (dentro de um país ou região) ou internacional (fora de um país ou região) com base no local do usuário.|
|destinationname|Cadeia de caracteres|País ou região discada.|
|ID|Cadeia de caracteres|ID da conferência de áudio.|
|licenseCapability|Cadeia de caracteres|A licença usada para a chamada.|
|inventorytype|Cadeia de caracteres|Tipo de número de telefone do usuário, como um serviço de número de chamada gratuita.|

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
