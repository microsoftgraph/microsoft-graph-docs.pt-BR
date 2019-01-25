---
title: tipo de recurso de scheduleInformation
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: e84505ee2f30a5b7b52e9d5b589b8bb24d9a4c95
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521905"
---
# <a name="scheduleinformation-resource-type"></a>tipo de recurso de scheduleInformation

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
 
Representa a disponibilidade de um usuário, uma lista de distribuição ou um recurso por um período de tempo especificado.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|availabilityView |String |Representa um modo de exibição mesclado de disponibilidade de todos os itens em `scheduleItems`. O modo de exibição consiste em intervalos de tempo. Disponibilidade durante cada intervalo de tempo é indicada com: `0`= gratuito, `1`= provisório, `2`= ocupado, `3`= ausência temporária, `4`= trabalhando em outros lugares.|
|erro |[freeBusyError](freebusyerror.md) |Informações de erro da tentativa de obter a disponibilidade do usuário, lista de distribuição ou recurso. |
|scheduleId |String |Um endereço SMTP do usuário, lista de distribuição ou recurso, que identifica uma instância de **scheduleInformation**. |
|scheduleItems |coleção [scheduleItem](scheduleitem.md) |Contém os itens que descrevem a disponibilidade do usuário ou recurso. |
|workingHours |[workingHours](workinghours.md) |Os dias da semana e as horas de um fuso horário específico que o usuário trabalha. Elas são definidas como parte do do usuário [mailboxSettings](mailboxsettings.md).|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scheduleInformation"
}-->

```json
{
  "availabilityView": "String",
  "error": {"@odata.type": "microsoft.graph.freeBusyError"},
  "scheduleId": "String",
  "scheduleItems": [{"@odata.type": "microsoft.graph.scheduleItem"}],
  "workingHours": {"@odata.type": "microsoft.graph.workingHours"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scheduleInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/scheduleinformation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
