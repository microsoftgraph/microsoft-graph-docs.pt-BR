---
title: tipo de recurso educationSynchronizationDataProvider
description: 'Representa o esquema SIS de origem. Isso permite que o sistema saiba como mapear os dados de entrada para o esquema do Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f592e75a3a6df1728839494ee41ac28065450d60
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507036"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>tipo de recurso educationSynchronizationDataProvider

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o esquema SIS de origem. Isso permite que o sistema saiba como mapear os dados de entrada para o esquema do Azure Active Directory (Azure AD).

> **Observação:** Esse tipo complexo é abstrato. Consulte os tipos específicos de provedores de dados listados.

## <a name="derived-types"></a>Tipos derivados
| Tipo | Descrição |
|:-|:-|:-|
| [educationcsvdataprovider](educationcsvdataprovider.md) | Usado com arquivos CSV como a fonte de entrada. |
| [educationpowerschooldataprovider](educationpowerschooldataprovider.md) | Usado com PowerSchool como a fonte de entrada. |
| [educationonerosterapidataprovider](educationonerosterapidataprovider.md) | Usado com a API OneRoster como a fonte de entrada. |

## <a name="properties"></a>Propriedades

Nenhuma propriedade é exposta por esse tipo.
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
