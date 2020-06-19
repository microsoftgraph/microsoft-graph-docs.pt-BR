---
title: tipo de recurso educationSynchronizationDataProvider
description: 'Representa o esquema SIS de origem. Isso permite que o sistema saiba como mapear os dados de entrada para o esquema do Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f0691a7157fb189e75e862448069ff8ebdeee9f7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790919"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>tipo de recurso educationSynchronizationDataProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o provedor de dados a ser usado como a fonte de sincronização de um [educationSynchronizationProfile].

> **Observação:** Esse tipo complexo é abstrato. Consulte os tipos específicos de provedores de dados listados.

## <a name="providers"></a>Provedores

| Data Provider                       | Descrição                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]          | Arquivos CSV carregados para a [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do perfil |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | API do OneRoster v 1.1                                                                                 |
| [educationPowerSchoolDataProvider]  | API da PowerSchool                                                                                    |

## <a name="properties"></a>Propriedades

Nenhuma propriedade é exposta por esse tipo.

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
