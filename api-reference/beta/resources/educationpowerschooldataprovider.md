---
title: recurso educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2469a99b8acbfa1bd4e5167cf67caa102fa9422e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507113"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="4d98f-103">recurso educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="4d98f-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d98f-104">Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="4d98f-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="4d98f-105">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="4d98f-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="4d98f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4d98f-106">Properties</span></span>

| <span data-ttu-id="4d98f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4d98f-107">Property</span></span> | <span data-ttu-id="4d98f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4d98f-108">Type</span></span> | <span data-ttu-id="4d98f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4d98f-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="4d98f-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="4d98f-110">**connectionUrl**</span></span> | <span data-ttu-id="4d98f-111">String</span><span class="sxs-lookup"><span data-stu-id="4d98f-111">String</span></span> | <span data-ttu-id="4d98f-112">A URL de conexão para a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="4d98f-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="4d98f-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="4d98f-113">**clientId**</span></span> | <span data-ttu-id="4d98f-114">String</span><span class="sxs-lookup"><span data-stu-id="4d98f-114">String</span></span> |  <span data-ttu-id="4d98f-115">A ID do cliente usada para se conectar ao PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="4d98f-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="4d98f-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="4d98f-116">**clientSecret**</span></span> | <span data-ttu-id="4d98f-117">String</span><span class="sxs-lookup"><span data-stu-id="4d98f-117">String</span></span> |  <span data-ttu-id="4d98f-118">O segredo do cliente para autenticar a conexão com a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="4d98f-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="4d98f-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="4d98f-119">**schoolsIds**</span></span> | <span data-ttu-id="4d98f-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="4d98f-120">String collection</span></span> |  <span data-ttu-id="4d98f-121">A lista de escolas a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="4d98f-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="4d98f-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="4d98f-122">**schoolYear**</span></span> | <span data-ttu-id="4d98f-123">String</span><span class="sxs-lookup"><span data-stu-id="4d98f-123">String</span></span> |  <span data-ttu-id="4d98f-124">O ano escolar a ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="4d98f-124">The school year to sync.</span></span> |
| <span data-ttu-id="4d98f-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="4d98f-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="4d98f-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="4d98f-126">Boolean</span></span> |  <span data-ttu-id="4d98f-127">Indica se a fonte tem vários identificadores para um único aluno ou professor.</span><span class="sxs-lookup"><span data-stu-id="4d98f-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="4d98f-128">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="4d98f-128">**customizations**</span></span> | [<span data-ttu-id="4d98f-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="4d98f-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="4d98f-130">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="4d98f-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4d98f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4d98f-131">JSON representation</span></span>
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
