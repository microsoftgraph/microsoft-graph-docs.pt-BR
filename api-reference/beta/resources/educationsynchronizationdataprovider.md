---
title: tipo de recurso educationSynchronizationDataProvider
description: 'Representa o esquema SIS de origem. Isso permite que o sistema saiba como mapear os dados de entrada para o esquema do Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: f20bea087a23f14acd7184c5211d21687409897a
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434967"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a>tipo de recurso educationSynchronizationDataProvider

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o provedor de dados a ser usado como a fonte de sincronização de um [educationSynchronizationProfile].

> [!NOTE]
> Esse tipo complexo é abstrato. Consulte os tipos específicos de provedores de dados listados.

## <a name="providers"></a>Provedores

| Data Provider                                                             | Descrição                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| [educationCsvDataProvider]                                                | Arquivos CSV carregados para a [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do perfil |
| [educationOneRosterApiDataProvider](educationonerosterapidataprovider.md) | API do OneRoster v 1.1                                                                                 |
| [educationPowerSchoolDataProvider]                                        | API da PowerSchool                                                                                    |

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
