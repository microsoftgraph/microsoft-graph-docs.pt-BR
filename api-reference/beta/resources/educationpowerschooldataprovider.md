---
title: recurso educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6a036435cb7cc1a4ef70960b09feb600fe7f39f8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972590"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="b7b5b-103">recurso educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="b7b5b-103">educationPowerSchoolDataProvider resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7b5b-104">Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-104">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="b7b5b-105">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="b7b5b-105">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b7b5b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7b5b-106">Properties</span></span>

| <span data-ttu-id="b7b5b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7b5b-107">Property</span></span> | <span data-ttu-id="b7b5b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7b5b-108">Type</span></span> | <span data-ttu-id="b7b5b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7b5b-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b7b5b-110">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-110">**connectionUrl**</span></span> | <span data-ttu-id="b7b5b-111">String</span><span class="sxs-lookup"><span data-stu-id="b7b5b-111">String</span></span> | <span data-ttu-id="b7b5b-112">A URL de conexão para a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-112">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="b7b5b-113">**clientId**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-113">**clientId**</span></span> | <span data-ttu-id="b7b5b-114">String</span><span class="sxs-lookup"><span data-stu-id="b7b5b-114">String</span></span> |  <span data-ttu-id="b7b5b-115">A ID do cliente usada para se conectar ao PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-115">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="b7b5b-116">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-116">**clientSecret**</span></span> | <span data-ttu-id="b7b5b-117">String</span><span class="sxs-lookup"><span data-stu-id="b7b5b-117">String</span></span> |  <span data-ttu-id="b7b5b-118">O segredo do cliente para autenticar a conexão com a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-118">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="b7b5b-119">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-119">**schoolsIds**</span></span> | <span data-ttu-id="b7b5b-120">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b7b5b-120">String collection</span></span> |  <span data-ttu-id="b7b5b-121">A lista de escolas a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-121">The list of schools to sync.</span></span> |
| <span data-ttu-id="b7b5b-122">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-122">**schoolYear**</span></span> | <span data-ttu-id="b7b5b-123">String</span><span class="sxs-lookup"><span data-stu-id="b7b5b-123">String</span></span> |  <span data-ttu-id="b7b5b-124">O ano escolar a ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-124">The school year to sync.</span></span> |
| <span data-ttu-id="b7b5b-125">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-125">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="b7b5b-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="b7b5b-126">Boolean</span></span> |  <span data-ttu-id="b7b5b-127">Indica se a fonte tem vários identificadores para um único aluno ou professor.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-127">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="b7b5b-128">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="b7b5b-128">**customizations**</span></span> | [<span data-ttu-id="b7b5b-129">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="b7b5b-129">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="b7b5b-130">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="b7b5b-130">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7b5b-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7b5b-131">JSON representation</span></span>
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
  "schoolsIds": ["String"],
  "schoolYear": "String",
  "allowTeachersInMultipleSchools": "Boolean",
  "customizations": {"@odata.type": "microsoft.graph.educationSynchronizationCustomizations"}
}
```
