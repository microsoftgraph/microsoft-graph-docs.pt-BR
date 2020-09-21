---
title: tipo de recurso educationSynchronizationDataProvider
description: 'Representa o esquema SIS de origem. Isso permite que o sistema saiba como mapear os dados de entrada para o esquema do Azure Active Directory (Azure AD). '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 952d0a7f9a40f41ad87d632386d9d567036cfec7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989649"
---
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="1b8f8-104">tipo de recurso educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="1b8f8-104">educationSynchronizationDataProvider resource type</span></span>

<span data-ttu-id="1b8f8-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b8f8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b8f8-106">Representa o provedor de dados a ser usado como a fonte de sincronização de um [educationSynchronizationProfile].</span><span class="sxs-lookup"><span data-stu-id="1b8f8-106">Represents the data provider to use as the synchronization source for a [educationSynchronizationProfile].</span></span>

> [!NOTE]
> <span data-ttu-id="1b8f8-107">Esse tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="1b8f8-107">This complex type is abstract.</span></span> <span data-ttu-id="1b8f8-108">Consulte os tipos específicos de provedores de dados listados.</span><span class="sxs-lookup"><span data-stu-id="1b8f8-108">Refer to the specific types of data providers listed.</span></span>

## <a name="providers"></a><span data-ttu-id="1b8f8-109">Provedores</span><span class="sxs-lookup"><span data-stu-id="1b8f8-109">Providers</span></span>

| <span data-ttu-id="1b8f8-110">Data Provider</span><span class="sxs-lookup"><span data-stu-id="1b8f8-110">Data Provider</span></span>                                                             | <span data-ttu-id="1b8f8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1b8f8-111">Description</span></span>                                                                                        |
| :------------------------------------------------------------------------ | :------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="1b8f8-112">[educationCsvDataProvider]</span><span class="sxs-lookup"><span data-stu-id="1b8f8-112">[educationCsvDataProvider]</span></span>                                                | <span data-ttu-id="1b8f8-113">Arquivos CSV carregados para a [URL SAS](../api/educationsynchronizationprofile-uploadurl.md) do perfil</span><span class="sxs-lookup"><span data-stu-id="1b8f8-113">CSV files uploaded to the Profile's [SAS URL](../api/educationsynchronizationprofile-uploadurl.md)</span></span> |
| [<span data-ttu-id="1b8f8-114">educationOneRosterApiDataProvider</span><span class="sxs-lookup"><span data-stu-id="1b8f8-114">educationOneRosterApiDataProvider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="1b8f8-115">API do OneRoster v 1.1</span><span class="sxs-lookup"><span data-stu-id="1b8f8-115">OneRoster v1.1 API</span></span>                                                                                 |
| <span data-ttu-id="1b8f8-116">[educationPowerSchoolDataProvider]</span><span class="sxs-lookup"><span data-stu-id="1b8f8-116">[educationPowerSchoolDataProvider]</span></span>                                        | <span data-ttu-id="1b8f8-117">API da PowerSchool</span><span class="sxs-lookup"><span data-stu-id="1b8f8-117">PowerSchool API</span></span>                                                                                    |

[educationsynchronizationprofile]: educationsynchronizationprofile.md
[educationcsvdataprovider]: educationCsvDataProvider.md
[educationsynchronizationdataprovider]: educationSynchronizationDataProvider.md
[educationpowerschooldataprovider]: educationPowerSchoolDataProvider.md
[educationcsvdataprovider]: educationCsvDataProvider.md


