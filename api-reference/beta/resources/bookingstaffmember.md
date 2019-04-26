---
title: tipo de recurso bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543724"
---
# <a name="bookingstaffmember-resource-type"></a>tipo de recurso bookingStaffMember

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um membro da equipe que fornece serviços em um [bookingBusiness](bookingbusiness.md).

Os membros da equipe podem fazer parte do locatário do Office 355 onde o negócio de reserva está configurado ou podem usar os serviços de email de outros provedores de email.

Ao reservar compromissos, a API Books considera as seguintes configurações para determinar a disponibilidade de um membro da equipe: 

1. Por padrão, as horas de operação da empresa (a propriedade **businessHours** da entidade [bookingBusiness](bookingbusiness.md) ) representam a disponibilidade geral do membro da equipe.
2. Se **useBusinessHours** for false, o horário de trabalho específico do membro da equipe (propriedade**WorkingHours** da entidade **bookingStaffmember** ) representará a disponibilidade geral do membro.
3. Se **availabilityIsAffectedByPersonalCalendar** for true, a API Books primeiro examinaria as horas do membro da equipe em geral (conforme determinado por #1 ou #2) e verificará a disponibilidade dessas horas no pessoal do membro da equipe calendário, antes de fazer uma reserva.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar membros da equipe](../api/bookingbusiness-list-staffmembers.md) | coleção [bookingStaffMember](bookingstaffmember.md) | Obtenha uma lista de objetos **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado. |
|[Criar bookingStaff](../api/bookingbusiness-post-staffmembers.md) | coleção [bookingStaffMember](bookingstaffmember.md) | Criar um novo **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado. |
|[Obter bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Obtenha as propriedades e os relacionamentos de um **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.|
|[Update](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |Atualiza as propriedades de um **bookingStaffMember** no [bookingbusiness](../resources/bookingbusiness.md)especificado.|
|[Excluir](../api/bookingstaffmember-delete.md) | None |Excluir um membro da equipe no [bookingbusiness](../resources/bookingbusiness.md)especificado. |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Booliano|True significa que, se o membro da equipe for um usuário do Office 365, a API de reservas verificará a disponibilidade do membro da equipe em seu calendário pessoal no Office 365, antes de fazer uma reserva. |
|colorIndex|Int32|Identifica uma cor para representar o membro da equipe. A cor corresponde à paleta de cores na página de **detalhes da equipe** no aplicativo de reservas.|
|displayName|Cadeia de caracteres|O nome do membro da equipe, conforme exibido para os clientes. Obrigatório.|
|emailAddress|String|O endereço de email do membro da equipe. Isso pode ser no mesmo locatário do Office 365 que a empresa ou em um domínio de email diferente. Esse endereço de email pode ser usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na política de agendamento da empresa. Obrigatório.|
|id|String| A ID do membro da equipe, em um formato GUID. Somente leitura.|
|role|string| A função do membro da equipe na empresa. Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`. Obrigatório.|
|useBusinessHours|Booliano|True significa que a disponibilidade do membro da equipe é conforme especificado na propriedade **businessHours** da empresa. False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours** do membro da equipe.|
|workingHours|coleção [bookingWorkHours](bookingworkhours.md)|O intervalo de horas por dia da semana em que o membro da equipe está disponível para reserva. Por padrão, eles são inicializados de acordo com a propriedade **businessHours** da empresa.|

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
  "workingHours": [{"@odata.type": "microsoft.graph.bookingWorkHours"}]
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
  "suppressions": [
    "Error: /api-reference/beta/resources/bookingstaffmember.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
