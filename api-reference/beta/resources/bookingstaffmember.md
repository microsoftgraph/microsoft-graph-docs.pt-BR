---
title: tipo de recurso de bookingStaffMember
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 72130f46dc67d4491f9855706528ee5894b8352f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520274"
---
# <a name="bookingstaffmember-resource-type"></a>tipo de recurso de bookingStaffMember

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa um membro da equipe que fornece serviços em um [bookingBusiness](bookingbusiness.md).

Membros da equipe podem fazer parte do inquilino 355 Office onde os negócios de reserva está configurado, ou eles podem usar os serviços de email de outros provedores de email.

Quando os compromissos de reserva, a API de reservas considera as configurações a seguir para determinar a disponibilidade de um membro da equipe: 

1. Por padrão, os horários de operação dos negócios (a propriedade **businessHours** da entidade [bookingBusiness](bookingbusiness.md) ) representa a disponibilidade geral do membro da equipe.
2. Se **useBusinessHours** for false, horas de trabalho específico do membro da equipe (**workingHours** de propriedade da entidade **bookingStaffmember** ) representa disponibilidade geral desse membro.
3. Se **availabilityIsAffectedByPersonalCalendar** for true, em seguida, a API de reservas seria primeiro examine do membro da equipe geralmente disponível em horas (conforme determinado pelo #1 ou 2 #) e verifique se disponibilidade durante os horários do pessoal do membro da equipe calendário, antes de fazer uma reserva.

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Membros da equipe de lista](../api/bookingbusiness-list-staffmembers.md) | coleção [bookingStaffMember](bookingstaffmember.md) | Obtenha uma lista de objetos **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md). |
|[Criar bookingStaff](../api/bookingbusiness-post-staffmembers.md) | coleção [bookingStaffMember](bookingstaffmember.md) | Crie um novo **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md). |
|[Obter bookingStaffMember](../api/bookingstaffmember-get.md) | [bookingStaffMember](bookingstaffmember.md) |Obtenha as propriedades e relacionamentos de um **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).|
|[Update](../api/bookingstaffmember-update.md) | [bookingStaffMember](bookingstaffmember.md)    |Atualize as propriedades de um **bookingStaffMember** no especificado [bookingbusiness](../resources/bookingbusiness.md).|
|[Delete](../api/bookingstaffmember-delete.md) | Nenhum |Exclua um membro da equipe no especificado [bookingbusiness](../resources/bookingbusiness.md). |

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityIsAffectedByPersonalCalendar|Booliano|True significa que se o membro da equipe é um usuário do Office 365, a API de reservas seria Verificar disponibilidade do membro da equipe no seu calendário pessoal no Office 365, antes de fazer uma reserva. |
|ColorIndex|Int32|Identifica uma cor para representar o membro da equipe. A cor corresponde à paleta de cores na página **detalhes da equipe** no aplicativo reservas.|
|displayName|String|O nome do membro da equipe, como exibido aos clientes. Obrigatório.|
|emailAddress|String|O endereço de email do membro da equipe. Isso pode ser em inquilino do Office 365 como a empresa ou em um domínio de email diferentes. Esse endereço de email pode ser usado se a propriedade **sendConfirmationsToOwner** estiver definida como true na diretiva de agendamento dos negócios. Obrigatório.|
|id|String| A identificação do membro da equipe, em um formato GUID. Somente leitura.|
|role|string| A função de membro da equipe de negócios. Os valores possíveis são: `guest`, `administrator`, `viewer`, `externalGuest`. Obrigatório.|
|useBusinessHours|Booliano|True significa disponibilidade do membro da equipe é como especificado na propriedade **businessHours** dos negócios. False significa que a disponibilidade é determinada pela configuração da propriedade **workingHours** do membro da equipe.|
|workingHours|coleção [bookingWorkHours](bookingworkhours.md)|O intervalo de horas por dia da semana em que o membro da equipe está disponível para marcação. Por padrão, eles são inicializados para ser o mesmo que a propriedade **businessHours** dos negócios.|

## <a name="relationships"></a>Relacionamento
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
