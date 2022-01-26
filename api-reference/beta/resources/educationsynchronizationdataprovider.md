---
title: tipo de recurso educationSynchronizationDataProvider
description: 'Representa o esquema SIS de origem. Isso permite que o sistema saiba como mapear os dados de entrada para o esquema Azure Active Directory (Azure AD). '
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 869b24f5db8619caf3d60c17538f7ed4f8d932a5
ms.sourcegitcommit: 871db8b3f68489d24e2aeafe694725579ee44c47
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2022
ms.locfileid: "62225753"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>tipo de recurso educationSynchronizationDataProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o provedor de dados a ser usado como fonte de sincronização para [um educationSynchronizationProfile].

> [!NOTE]
> Esse tipo complexo é abstrato. Consulte os tipos específicos de provedores de dados listados.


**Provedores**

| Data Provider                                                             | Descrição                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | Arquivos CSV carregados na [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do Perfil |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | OneRoster v1.1 API                                                                                 |
| [educationPowerSchoolDataProvider]                                        | API da PowerSchool                                                                                    |

## <a name="properties"></a>Propriedades

Nenhum.

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationDataProvider"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationDataProvider"
}
```


[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
