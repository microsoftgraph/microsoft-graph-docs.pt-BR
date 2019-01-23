---
title: tipo de recurso de educationSynchronizationDataProvider
description: 'Representa o esquema SIS de origem. Isso permite que o sistema para saber como mapear os dados de entrada para o esquema do Active Directory (AD Azure) do Azure. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f1e51bd0039b28aa08fa71956efc5143df77651c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420966"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>tipo de recurso de educationSynchronizationDataProvider

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

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



<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationDataProvider "
}-->

```json
{
}
```
