---
title: recurso de educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510460"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="f5957-103">recurso de educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="f5957-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5957-104">Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="f5957-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="f5957-105">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="f5957-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f5957-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5957-106">Properties</span></span>

| <span data-ttu-id="f5957-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5957-107">Property</span></span> | <span data-ttu-id="f5957-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5957-108">Type</span></span> | <span data-ttu-id="f5957-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5957-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f5957-110">**URL de conexão**</span><span class="sxs-lookup"><span data-stu-id="f5957-110">**connectionUrl**</span></span> | <span data-ttu-id="f5957-111">String</span><span class="sxs-lookup"><span data-stu-id="f5957-111">String</span></span> | <span data-ttu-id="f5957-112">A URL da conexão para a instância de PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="f5957-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="f5957-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="f5957-113">**clientId**</span></span> | <span data-ttu-id="f5957-114">String</span><span class="sxs-lookup"><span data-stu-id="f5957-114">String</span></span> |  <span data-ttu-id="f5957-115">A identificação do cliente usada para conectar ao PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="f5957-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="f5957-116">client_secret</span><span class="sxs-lookup"><span data-stu-id="f5957-116">**clientSecret**</span></span> | <span data-ttu-id="f5957-117">String</span><span class="sxs-lookup"><span data-stu-id="f5957-117">String</span></span> |  <span data-ttu-id="f5957-118">O segredo do cliente para autenticar a conexão à instância PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="f5957-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="f5957-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="f5957-119">**schoolsIds**</span></span> | <span data-ttu-id="f5957-120">String collection</span><span class="sxs-lookup"><span data-stu-id="f5957-120">String collection</span></span> |  <span data-ttu-id="f5957-121">A lista de escolas para sincronizar.</span><span class="sxs-lookup"><span data-stu-id="f5957-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="f5957-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="f5957-122">**schoolYear**</span></span> | <span data-ttu-id="f5957-123">String</span><span class="sxs-lookup"><span data-stu-id="f5957-123">String</span></span> |  <span data-ttu-id="f5957-124">O ano escola para sincronizar.</span><span class="sxs-lookup"><span data-stu-id="f5957-124">The school year to sync.</span></span> |
| <span data-ttu-id="f5957-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="f5957-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="f5957-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5957-126">Boolean</span></span> |  <span data-ttu-id="f5957-127">Indica se a fonte tem vários identificadores para um único aluno ou professor.</span><span class="sxs-lookup"><span data-stu-id="f5957-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="f5957-128">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="f5957-128">**customizations**</span></span> | [<span data-ttu-id="f5957-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="f5957-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="f5957-130">Personalização opcional a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="f5957-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5957-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5957-131">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider"
}-->

```json
{
    "@odata.type": "microsoft.graph.educationPowerSchoolDataProvider",
    "connectionUrl": "String",
    "clientId": "String",
    "clientSecret": "String",
    "schoolsids": ["String"],
    "schoolYear": "String",
    "allowTeachersInMultipleSchools": "Boolean",
    "customizations": { "@odata.type": "microsoft.graph.educationSynchronizationCustomizations" }
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerschooldataprovider.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
