---
title: Tipo de recurso bookingStaffMember
description: Representa um membro da equipe que fornece serviços em um bookingBusiness.
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 25569646633195e9cbce1067dad1abbd369885a2
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160619"
---
# <a name="bookingstaffmember-resource-type"></a>Tipo de recurso bookingStaffMember

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um membro da equipe que fornece serviços em um [bookingBusiness](bookingbusiness.md).

Os membros da equipe podem fazer parte do locatário Microsoft 365 local em que a empresa de reserva está configurada ou podem usar serviços de email de outros provedores de email.

Ao reservar compromissos, a API do Bookings considera as seguintes configurações para determinar a disponibilidade de um membro da equipe: 

1. Por padrão, as horas de operação da empresa (a propriedade **businessHours** da entidade [bookingBusiness](bookingbusiness.md) ) representam a disponibilidade geral do membro da equipe.
2. Se **useBusinessHours** for false, as horas de trabalho específicas do membro da equipe (propriedade **workingHours** da entidade **bookingStaffmember** ) representarão a disponibilidade geral desse membro.
3. Se **availabilityIsAffectedByPersonalCalendar** for verdadeira, a API do Bookings primeiro examinará as horas geralmente disponíveis do membro da equipe (conforme determinado pelo nº 1 ou nº 2) e verificará a disponibilidade durante essas horas no calendário pessoal do membro da equipe, antes de fazer uma reserva.

Microsoft Bookings dá suporte a no máximo 100 membros da equipe em um calendário de reserva.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar membros da equipe](../api/bookingbusiness-list-staffmembers.md) | [coleção bookingStaffMember](bookingstaffmember.md) | Obtenha uma lista de **objetos bookingStaffMember** no [bookingbusiness especificado](../resources/bookingbusiness.md). |
|[Criar bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [coleção bookingStaffMember](bookingstaffmember.md) | Crie um **novo bookingStaffMember** no [bookingbusiness especificado](../resources/bookingbusiness.md). |
|[Obter bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Obtenha as propriedades e as relações de **um bookingStaffMember** no [bookingbusiness especificado](../resources/bookingbusiness.md).|
|[Atualizar](../api/bookingstaffmember-update.md) | Nenhum(a)   |Atualize as propriedades de **um bookingStaffMember** no [bookingbusiness especificado](../resources/bookingbusiness.md).|
|[Excluir](../api/bookingstaffmember-delete.md) | Nenhuma |Exclua um membro da equipe no [bookingbusiness especificado](../resources/bookingbusiness.md). |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Boolean|True significa que, se o membro da equipe for um Microsoft 365 usuário, a API do Bookings verificaria a disponibilidade do membro da equipe em seu calendário pessoal em Microsoft 365, antes de fazer uma reserva. |
|colorIndex|Int32|Identifica uma cor para representar o membro da equipe. A cor corresponde à paleta de cores na página **Detalhes da** equipe no aplicativo Bookings.|
|displayName|Cadeia de caracteres|O nome do membro da equipe, conforme exibido aos clientes. Obrigatório.|
|emailAddress|String|O endereço de email do membro da equipe. Isso pode estar no mesmo locatário Microsoft 365 que a empresa ou em um domínio de email diferente. Esse endereço de email poderá ser usado se **a propriedade sendConfirmationsToOwner** estiver definida como true na política de agendamento da empresa. Obrigatório.|
|id|Cadeia de caracteres| A ID do membro da equipe, em um formato GUID. Somente leitura.|
|IsEmailNotificationEnabled|Boolean|`True` significa que o membro da equipe será notificado por email quando uma reserva atribuída a ele for criada ou alterada.
|role|bookingStaffRole| A função do membro da equipe na empresa. Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`, `unknownFutureValue`e `scheduler` `member`. Observe que você deve usar o `Prefer: include-unknown-enum-members` cabeçalho da solicitação para obter os seguintes valores neste `[evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)`: `scheduler`, `member`. Obrigatório. |
|timeZone|Cadeia de caracteres|O fuso horário do membro da equipe. Para obter uma lista de valores possíveis, consulte [dateTimeTimeZone](datetimetimezone.md).|
|useBusinessHours|Boolean|True significa que a disponibilidade do membro da equipe é conforme especificado na **propriedade businessHours** da empresa. False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours do** membro da equipe.|
|workingHours|[coleção bookingWorkHours](bookingworkhours.md)|O intervalo de horas a cada dia da semana em que o membro da equipe está disponível para reserva. Por padrão, eles são inicializados para serem iguais à propriedade **businessHours** da empresa.|

## <a name="relationships"></a>Relações
Nenhum


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.bookingStaffMember"
}-->

```json
{
  "availabilityIsAffectedByPersonalCalendar": true,
  "colorIndex": 1024,
  "displayName": "String",
  "emailAddress": "String",
  "id": "String (identifier)",
  "role": {"@odata.type": "microsoft.graph.bookingStaffRole"},
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "timeZone": "String",
  "IsEmailNotificationEnabled": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingStaffMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


