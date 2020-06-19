---
title: recurso educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9b85870f44eae936411e2aacf71781876858eee3
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790940"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="e6efe-103">recurso educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="e6efe-103">educationPowerSchoolDataProvider resource</span></span>

<span data-ttu-id="e6efe-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6efe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6efe-105">Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="e6efe-105">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="e6efe-106">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="e6efe-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e6efe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6efe-107">Properties</span></span>

| <span data-ttu-id="e6efe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6efe-108">Property</span></span>                       | <span data-ttu-id="e6efe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6efe-109">Type</span></span>                                     | <span data-ttu-id="e6efe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6efe-110">Description</span></span>                                                                            |
| :----------------------------- | :--------------------------------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="e6efe-111">allowTeachersInMultipleSchools</span><span class="sxs-lookup"><span data-stu-id="e6efe-111">allowTeachersInMultipleSchools</span></span> | <span data-ttu-id="e6efe-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6efe-112">Boolean</span></span>                                  | <span data-ttu-id="e6efe-113">Indica se a fonte tem vários identificadores para um único aluno ou professor.</span><span class="sxs-lookup"><span data-stu-id="e6efe-113">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="e6efe-114">clientId</span><span class="sxs-lookup"><span data-stu-id="e6efe-114">clientId</span></span>                       | <span data-ttu-id="e6efe-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6efe-115">String</span></span>                                   | <span data-ttu-id="e6efe-116">A ID do cliente usada para se conectar ao PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="e6efe-116">The client ID used to connect to PowerSchool.</span></span>                                          |
| <span data-ttu-id="e6efe-117">clientSecret</span><span class="sxs-lookup"><span data-stu-id="e6efe-117">clientSecret</span></span>                   | <span data-ttu-id="e6efe-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6efe-118">String</span></span>                                   | <span data-ttu-id="e6efe-119">O segredo do cliente para autenticar a conexão com a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="e6efe-119">The client secret to authenticate the connection to the PowerSchool instance.</span></span>          |
| <span data-ttu-id="e6efe-120">connectionUrl</span><span class="sxs-lookup"><span data-stu-id="e6efe-120">connectionUrl</span></span>                  | <span data-ttu-id="e6efe-121">String</span><span class="sxs-lookup"><span data-stu-id="e6efe-121">String</span></span>                                   | <span data-ttu-id="e6efe-122">A URL de conexão para a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="e6efe-122">The connection URL to the PowerSchool instance.</span></span>                                        |
| <span data-ttu-id="e6efe-123">schoolsIds</span><span class="sxs-lookup"><span data-stu-id="e6efe-123">schoolsIds</span></span>                     | <span data-ttu-id="e6efe-124">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6efe-124">String collection</span></span>                        | <span data-ttu-id="e6efe-125">A lista de escolas a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="e6efe-125">The list of schools to sync.</span></span>                                                           |
| <span data-ttu-id="e6efe-126">schoolYear</span><span class="sxs-lookup"><span data-stu-id="e6efe-126">schoolYear</span></span>                     | <span data-ttu-id="e6efe-127">String</span><span class="sxs-lookup"><span data-stu-id="e6efe-127">String</span></span>                                   | <span data-ttu-id="e6efe-128">O ano escolar a ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="e6efe-128">The school year to sync.</span></span>                                                               |
| <span data-ttu-id="e6efe-129">personalizações</span><span class="sxs-lookup"><span data-stu-id="e6efe-129">customizations</span></span>                 | <span data-ttu-id="e6efe-130">[educationSynchronizationCustomizations]</span><span class="sxs-lookup"><span data-stu-id="e6efe-130">[educationSynchronizationCustomizations]</span></span> | <span data-ttu-id="e6efe-131">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="e6efe-131">Optional customization to be applied to the synchronization profile.</span></span>                   |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md
[educationsynchronizationcustomizations]: educationsynchronizationcustomizations.md

## <a name="json-representation"></a><span data-ttu-id="e6efe-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6efe-133">JSON representation</span></span>

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
  "customizations": {
    "@odata.type": "microsoft.graph.educationSynchronizationCustomizations"
  }
}
```
