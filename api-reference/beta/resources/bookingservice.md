---
title: Tipo de recurso bookingService
description: Representa informações sobre um serviço específico fornecido por um bookingBusiness, como o nome do serviço, o preço e a equipe que geralmente fornece esse serviço.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d8c8fb849bbc452d343cb37b86e8cfae925606ae
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160703"
---
# <a name="bookingservice-resource-type"></a>Tipo de recurso bookingService

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa informações sobre um serviço específico fornecido por um [bookingBusiness](bookingbusiness.md), como o nome do serviço, o preço e a equipe que geralmente fornece esse serviço.

Herda de [bookingNamedEntity](bookingNamedEntity.md).

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar serviços](../api/bookingbusiness-list-services.md) | [coleção bookingService](bookingservice.md) | Obtenha uma lista de **objetos bookingService** no [bookingbusiness especificado](../resources/bookingbusiness.md).|
|[Criar bookingService](../api/bookingbusiness-post-services.md) | [bookingService](bookingservice.md) | Crie um **bookingService** para o [bookingbusiness especificado](../resources/bookingbusiness.md). |
|[Obter bookingService](../api/bookingservice-get.md) | [bookingService](bookingservice.md) |Obtenha as propriedades e as relações de um **objeto bookingService** no [bookingbusiness especificado](../resources/bookingbusiness.md).|
|[Atualizar](../api/bookingservice-update.md) | Nenhum(a)   |Atualize **um objeto bookingService** no [bookingbusiness especificado](../resources/bookingbusiness.md). |
|[Excluir](../api/bookingservice-delete.md) | Nenhuma |**Exclua um objeto bookingService** no [bookingbusiness especificado](../resources/bookingbusiness.md). |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|additionalInformation|Cadeia de Caracteres|Informações adicionais que são enviadas ao cliente quando um compromisso é confirmado.|
|customQuestions|[coleção bookingQuestionAssignment](../resources/bookingquestionassignment.md)| Contém o conjunto de perguntas personalizadas associadas a um serviço específico. |
|defaultDuration|Duration|O comprimento padrão do serviço, representado em números de dias, horas, minutos e segundos. Por exemplo, P11D23H59M59.999999999999S. |
|Defaultlocation|[location](location.md)|O local físico padrão para o serviço.|
|defaultPrice|Duplo|O preço monetário padrão para o serviço.|
|defaultPriceType|bookingPriceType|A maneira padrão como o serviço é cobrado. Os valores possíveis são: `undefined`, `fixedPrice`, `startingAt`, `hourly`, `free`, `priceVaries`, `callUs`, `notSet`, `unknownFutureValue`.|
|defaultReminders|[coleção bookingReminder](bookingreminder.md)|O conjunto padrão de lembretes para um compromisso desse serviço. O valor dessa propriedade está disponível somente ao ler este **bookingService** por sua ID.|
|description|Cadeia de caracteres|Uma descrição de texto para o serviço.|
|displayName|Cadeia de caracteres|Um nome de serviço.|
|id|Cadeia de caracteres|A ID desse serviço, em um formato GUID. Somente leitura.|
|isAnonymousJoinEnabled|Boolean|`True` se um anonymousJoinWebUrl(webrtcUrl) for gerado para o compromisso reservado para esse serviço.
|isHiddenFromCustomers|Boolean|True significa que esse serviço não está disponível para os clientes para reserva.|
|isLocationOnline|Boolean|True indica que os compromissos para o serviço serão mantidos online. O valor padrão é falso.|
|languageTag|Cadeia de Caracteres|O idioma da página de reserva de autoatendimento.
|maximumAttendeesCount|Int32|O número máximo de clientes permitidos em um serviço. Se **maximumAttendeesCount** do serviço for maior que 1, passe as IDs de cliente válidas ao criar ou atualizar um compromisso.  Para criar um cliente, use a [operação Criar bookingCustomer](../api/bookingbusiness-post-customers.md) .  |
|notes|String|Informações adicionais sobre esse serviço.|
|Postbuffer|Duration|O tempo para armazenar em buffer após um compromisso para esse serviço termina e antes que o próximo compromisso do cliente possa ser reservado.|
|Prebuffer|Duration|O tempo para armazenar em buffer antes que um compromisso para esse serviço possa ser iniciado.|
|schedulingPolicy|[bookingSchedulingPolicy](bookingschedulingpolicy.md)|O conjunto de políticas que determinam como os compromissos para esse tipo de serviço devem ser criados e gerenciados.|
|smsNotificationsEnabled|Boolean|True indica SMS notificações podem ser enviadas aos clientes para o compromisso do serviço. O valor padrão é falso.|
|staffMemberIds|Coleção de cadeias de caracteres|Representa os [membros da equipe](bookingstaffmember.md) que fornecem esse serviço. |
|webUrl|String|A URL que um cliente usa para acessar o serviço.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingService"
}-->

```json
{
  "additionalInformation": "String",
  "defaultDuration": "String (timestamp)",
  "defaultLocation": {"@odata.type": "microsoft.graph.location"},
  "defaultPrice": 1024,
  "defaultPriceType": {"@odata.type": "microsoft.graph.bookingPriceType"},
  "defaultReminders": [{"@odata.type": "microsoft.graph.bookingReminder"}],
  "description": "String",
  "displayName": "String",
  "id": "String (identifier)",
  "languageTag": "String",
  "isHiddenFromCustomers": true,
  "isLocationOnline": "Boolean",
  "notes": "String",
  "postBuffer": "String (timestamp)",
  "preBuffer": "String (timestamp)",
  "schedulingPolicy": {"@odata.type": "microsoft.graph.bookingSchedulingPolicy"},
  "smsNotificationsEnabled": "Boolean",
  "staffMemberIds": ["String"],
  "customQuestions": [
    {
      "@odata.type": "microsoft.graph.bookingQuestionAssignment"
    }
  ],
  "maximumAttendeesCount": "Integer",
  "isAnonymousJoinEnabled": "Boolean",
  "webUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingService resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


