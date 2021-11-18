---
title: Tipo de recurso bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.localizationpriority: medium
author: arvindmicrosoft
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: d31705bb569037f73053c2a9b07e0bc93d5a1d60
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61077261"
---
# <a name="bookingstaffmember-resource-type"></a>Tipo de recurso bookingStaffMember

Namespace: microsoft.graph

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um membro da equipe que fornece serviços em [um bookingBusiness](bookingbusiness.md).

Os membros da equipe podem fazer parte do Microsoft 365 locatário em que a empresa de reserva está configurada ou podem usar serviços de email de outros provedores de email.

Ao reservar compromissos, a API do Bookings considera as seguintes configurações para determinar a disponibilidade de um membro da equipe: 

1. Por padrão, os horários de operação da empresa (a **propriedade businessHours** da [entidade bookingBusiness)](bookingbusiness.md) representam a disponibilidade geral do membro da equipe.
2. Se **useBusinessHours** for false, as horas de trabalho específicas do membro da equipe (**propriedade workingHours** da **entidade bookingStaffmember)** representam a disponibilidade geral desse membro.
3. Se **availabilityIsAffectedByPersonalCalendar** for true, a API do Bookings primeiro olharia para os horários geralmente disponíveis do membro da equipe (conforme determinado pelo #1 ou #2) e verificaria a disponibilidade durante essas horas no calendário pessoal do membro da equipe, antes de fazer uma reserva.

## <a name="methods"></a>Methods

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar membros da equipe](../api/bookingbusiness-list-staffmembers.md) | [coleção bookingStaffMember](bookingstaffmember.md) | Obter uma lista de **objetos bookingStaffMember** no [bookingbusiness especificado.](../resources/bookingbusiness.md) |
|[Criar bookingStaff](../api/bookingbusiness-post-staffmembers.md) | [coleção bookingStaffMember](bookingstaffmember.md) | Crie um novo **bookingStaffMember** no [bookingbusiness especificado.](../resources/bookingbusiness.md) |
|[Obter bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Obter as propriedades e relações de **um bookingStaffMember** no [bookingbusiness especificado.](../resources/bookingbusiness.md)|
|[Atualização](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |Atualize as propriedades de **um bookingStaffMember** no [bookingbusiness especificado.](../resources/bookingbusiness.md)|
|[Delete](../api/bookingstaffmember-delete.md) | Nenhum |Exclua um membro da equipe no [bookingbusiness especificado.](../resources/bookingbusiness.md) |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Booliano|True significa que, se o membro da equipe for um usuário Microsoft 365, a API do Bookings verificaria a disponibilidade do membro da equipe em seu calendário pessoal no Microsoft 365, antes de fazer uma reserva. |
|colorIndex|Int32|Identifica uma cor para representar o membro da equipe. A cor corresponde à paleta de cores na página **Detalhes da** Equipe no aplicativo Bookings.|
|displayName|String|O nome do membro da equipe, conforme exibido para os clientes. Obrigatório.|
|emailAddress|String|O endereço de email do membro da equipe. Isso pode estar no mesmo Microsoft 365 locatário que a empresa ou em um domínio de email diferente. Esse endereço de email pode ser usado **se a propriedade sendConfirmationsToOwner** estiver definida como true na política de agendamento da empresa. Obrigatório.|
|id|Cadeia de caracteres| A ID do membro da equipe, em um formato GUID. Somente leitura.|
|role|string| A função do membro da equipe na empresa. Os valores possíveis são: `guest` , , , , e `administrator` `viewer` `externalGuest` `scheduler` `member` . Obrigatório.|
|timeZone|Cadeia de caracteres|O fuso horário do membro da equipe. Para uma lista de valores possíveis, consulte [dateTimeTimeZone](datetimetimezone.md).|
|useBusinessHours|Boolean|True significa que a disponibilidade do membro da equipe está conforme especificado na **propriedade businessHours** da empresa. False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours** do membro da equipe.|
|workingHours|[Coleção bookingWorkHours](bookingworkhours.md)|O intervalo de horas a cada dia da semana que o membro da equipe está disponível para reserva. Por padrão, eles são inicializados para serem iguais à **propriedade businessHours** da empresa.|

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
  "role": "string",
  "useBusinessHours": true,
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}],
  "timeZone": "String"
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


