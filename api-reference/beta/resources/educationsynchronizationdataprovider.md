---
title: tipo de recurso de educationSynchronizationDataProvider
description: 'Representa o esquema SIS de origem. Isso permite que o sistema para saber como mapear os dados de entrada para o esquema do Active Directory (AD Azure) do Azure. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515493"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>tipo de recurso de educationSynchronizationDataProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o esquema SIS de origem. Isso permite que o sistema para saber como mapear os dados de entrada para o esquema do Active Directory (AD Azure) do Azure.

> **Observação:** Este tipo complexo é abstrato. Consulte os tipos específicos de provedores de dados listados.

## <a name="derived-types"></a>Tipos derivados
| Tipo | Descrição |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | Usada com arquivos CSV como a fonte de entrada. |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | Usada com PowerSchool como a fonte de entrada. |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | Usada com a API de OneRoster como a fonte de entrada. |

## <a name="properties"></a>Propriedades

Não há propriedades são expostas por esse tipo.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
