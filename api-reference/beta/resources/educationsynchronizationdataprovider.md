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
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="9d5a8-104">tipo de recurso educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="9d5a8-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="9d5a8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d5a8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d5a8-106">Representa o provedor de dados a ser usado como a fonte de sincronização de um [educationSynchronizationProfile].</span><span class="sxs-lookup"><span data-stu-id="9d5a8-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> <span data-ttu-id="9d5a8-107">**Observação:** Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="9d5a8-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="9d5a8-108">Consulte os tipos específicos de provedores de dados listados.</span><span class="sxs-lookup"><span data-stu-id="9d5a8-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="9d5a8-109">Provedores</span><span class="sxs-lookup"><span data-stu-id="9d5a8-109">Providers</span></span>

| <span data-ttu-id="9d5a8-110">Data Provider</span><span class="sxs-lookup"><span data-stu-id="9d5a8-110">Data Provider</span></span>                       | <span data-ttu-id="9d5a8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d5a8-111">Description</span></span>                                                                                        |
| :---------------------------------- | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="9d5a8-112">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="9d5a8-112">[educationCsvDataProvider]</span></span>          | <span data-ttu-id="9d5a8-113">Arquivos CSV carregados para a [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do perfil</span><span class="sxs-lookup"><span data-stu-id="9d5a8-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="9d5a8-114">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="9d5a8-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="9d5a8-115">API do OneRoster v 1.1</span><span class="sxs-lookup"><span data-stu-id="9d5a8-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="9d5a8-116">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="9d5a8-116">[educationPowerSchoolDataProvider]</span></span>  | <span data-ttu-id="9d5a8-117">API da PowerSchool</span><span class="sxs-lookup"><span data-stu-id="9d5a8-117">PowerSchool API</span></span>                                                                                    |

## <a name="properties"></a><span data-ttu-id="9d5a8-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d5a8-118">Properties</span></span>

<span data-ttu-id="9d5a8-119">Nenhuma propriedade é exposta por esse tipo.</span><span class="sxs-lookup"><span data-stu-id="9d5a8-119">No properties are exposed by this type.</span></span>

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md
