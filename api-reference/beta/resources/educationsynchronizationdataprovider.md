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
# <a name="educationsynchronizationdataprovider-resource-type"></a><span data-ttu-id="4bec0-104">tipo de recurso de educationSynchronizationDataProvider</span><span class="sxs-lookup"><span data-stu-id="4bec0-104">educationSynchronizationDataProvider resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4bec0-105">Representa o esquema SIS de origem.</span><span class="sxs-lookup"><span data-stu-id="4bec0-105">Represents the source SIS schema.</span></span> <span data-ttu-id="4bec0-106">Isso permite que o sistema para saber como mapear os dados de entrada para o esquema do Active Directory (AD Azure) do Azure.</span><span class="sxs-lookup"><span data-stu-id="4bec0-106">This allows the system to know how to map the incoming data to the Azure Active Directory (Azure AD) schema.</span></span>

> <span data-ttu-id="4bec0-107">**Observação:** Este tipo complexo é abstrato.</span><span class="sxs-lookup"><span data-stu-id="4bec0-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="4bec0-108">Consulte os tipos específicos de provedores de dados listados.</span><span class="sxs-lookup"><span data-stu-id="4bec0-108">Refer to the specific types of data providers listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="4bec0-109">Tipos derivados</span><span class="sxs-lookup"><span data-stu-id="4bec0-109">Derived types</span></span>
| <span data-ttu-id="4bec0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bec0-110">Type</span></span> | <span data-ttu-id="4bec0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bec0-111">Description</span></span> |
|:-|:-|:-|
| [<span data-ttu-id="4bec0-112">educationcsvdataprovider</span><span class="sxs-lookup"><span data-stu-id="4bec0-112">educationcsvdataprovider</span></span>](educationcsvdataprovider.md) | <span data-ttu-id="4bec0-113">Usada com arquivos CSV como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="4bec0-113">Used with CSV files as the input source.</span></span> |
| [<span data-ttu-id="4bec0-114">educationpowerschooldataprovider</span><span class="sxs-lookup"><span data-stu-id="4bec0-114">educationpowerschooldataprovider</span></span>](educationpowerschooldataprovider.md) | <span data-ttu-id="4bec0-115">Usada com PowerSchool como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="4bec0-115">Used with PowerSchool as the input source.</span></span> |
| [<span data-ttu-id="4bec0-116">educationonerosterapidataprovider</span><span class="sxs-lookup"><span data-stu-id="4bec0-116">educationonerosterapidataprovider</span></span>](educationonerosterapidataprovider.md) | <span data-ttu-id="4bec0-117">Usada com a API de OneRoster como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="4bec0-117">Used with OneRoster API as the input source.</span></span> |

## <a name="properties"></a><span data-ttu-id="4bec0-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bec0-118">Properties</span></span>

<span data-ttu-id="4bec0-119">Não há propriedades são expostas por esse tipo.</span><span class="sxs-lookup"><span data-stu-id="4bec0-119">No properties are exposed by this type.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationdataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
