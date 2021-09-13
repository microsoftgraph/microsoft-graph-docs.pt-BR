---
title: Tipo de recurso pstnCallLogRow
description: Representa uma linha de dados no log de chamadas PSTN (Rede Telefônica pública de Comutr).
author: williamlooney
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2a4d14df3b46e4a31d74b2f3a0cf2e111e7d1bc0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113816"
---
# <a name="pstncalllogrow-resource-type"></a>Tipo de recurso pstnCallLogRow

Namespace: microsoft.graph.callRecords

Representa uma linha de dados no log de chamadas PSTN (Rede Telefônica pública de Comutr). Cada linha mapeia para uma chamada.

## <a name="methods"></a>Métodos

| Método       | Tipo de retorno | Descrição |
|:-------------|:------------|:------------|
| [getPstnCalls](../api/callrecords-callrecord-getpstncalls.md) | [coleção microsoft.graph.callRecords.pstnCallLogRow](callrecords-pstncalllogrow.md) | Listar **objetos pstnCallLogRow** em um registro de chamada. |

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|callDurationSource|microsoft.graph.callRecords.pstnCallDurationSource|A origem dos dados de duração da chamada. Se a chamada usar um operador de telecomunicações de terceiros por meio do Programa Conexão Operador, o operador poderá fornecer seus próprios dados de duração da chamada. Nesse caso, o valor da propriedade é `operator` . Caso contrário, o valor será `microsoft` .|
|calleeNumber|String|Número discado no [formato E.164.](https://en.wikipedia.org/wiki/E.164)|
|callerNumber|String|Número que recebeu a chamada para chamadas de entrada ou o número discado para chamadas de saída. Formato E.164.|
|callId|String|Identificador de chamada. Não é garantido que seja exclusivo.|
|callType|String|Se a chamada foi uma chamada de saída ou de entrada PSTN e o tipo de chamada, como uma chamada feita por um usuário ou uma conferência de áudio.|
|charge|Duplo|Quantidade de dinheiro ou custo da chamada que é cobrada em sua conta.|
|conferenceId|String|ID da conferência de áudio.|
|connectionCharge|Duplo|Preço da taxa de conexão.|
|currency|String|Tipo de moeda usada para calcular o custo da chamada ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217)).|
|destinationContext|String|Se a chamada foi doméstica (dentro de um país ou região) ou internacional (fora de um país ou região) com base na localização do usuário.|
|destinationName|Cadeia de caracteres|País ou região discada.|
|duração|Int32|Por quanto tempo a chamada foi conectada, em segundos.|
|endDateTime|DateTimeOffset|Hora da finalização da chamada.|
|id|Cadeia de caracteres|Identificador de chamada exclusivo. GUID.|
|inventoryType|String|Tipo de número de telefone do usuário, como um serviço de número de chamada gratuita.|
|licenseCapability|Cadeia de caracteres|A licença usada para a chamada.|
|operator|Cadeia de caracteres|O operador de telecomunicações que forneceu serviços PSTN para essa chamada. Pode ser a Microsoft ou pode ser um operador de terceiros por meio do [Programa Conexão Operador.](https://techcommunity.microsoft.com/t5/microsoft-teams-blog/introducing-operator-connect-and-more-teams-calling-updates/ba-p/2176398)|
|startDateTime|DateTimeOffset|Hora do início da chamada.|
|tenantCountryCode|Cadeia de caracteres|Código de país do locatário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|usageCountryCode|Cadeia de caracteres|Código de país do usuário, [ISO 3166-1 alfa-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).|
|userDisplayName|Cadeia de caracteres|Nome de exibição do usuário.|
|userId|Cadeia de caracteres|Chamando a ID do usuário Graph. GUID. Essa e outras informações de usuário serão nulas/vazias para tipos de chamada de bot (ucap_in, ucap_out).|
|userPrincipalName|Cadeia de caracteres|UserPrincipalName (nome de login) no Azure Active Directory. Isso geralmente é o mesmo que o Endereço SIP do usuário e pode ser igual ao endereço de email do usuário.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
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
  "inventoryType": "String",
  "operator": "String",
  "callDurationSource": "String"
}
```


