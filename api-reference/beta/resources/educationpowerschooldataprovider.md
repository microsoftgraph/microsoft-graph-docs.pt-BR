---
title: recurso educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4fda7cc98c8041aad45a0ef8453affc9af34edc5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42501224"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="7b180-103">recurso educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="7b180-103">educationPowerSchoolDataProvider resource</span></span>

<span data-ttu-id="7b180-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7b180-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b180-105">Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="7b180-105">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="7b180-106">Derivado de [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="7b180-106">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7b180-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7b180-107">Properties</span></span>

| <span data-ttu-id="7b180-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7b180-108">Property</span></span> | <span data-ttu-id="7b180-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7b180-109">Type</span></span> | <span data-ttu-id="7b180-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7b180-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7b180-111">**connectionUrl**</span><span class="sxs-lookup"><span data-stu-id="7b180-111">**connectionUrl**</span></span> | <span data-ttu-id="7b180-112">String</span><span class="sxs-lookup"><span data-stu-id="7b180-112">String</span></span> | <span data-ttu-id="7b180-113">A URL de conexão para a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="7b180-113">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="7b180-114">**clientId**</span><span class="sxs-lookup"><span data-stu-id="7b180-114">**clientId**</span></span> | <span data-ttu-id="7b180-115">String</span><span class="sxs-lookup"><span data-stu-id="7b180-115">String</span></span> |  <span data-ttu-id="7b180-116">A ID do cliente usada para se conectar ao PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="7b180-116">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="7b180-117">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="7b180-117">**clientSecret**</span></span> | <span data-ttu-id="7b180-118">String</span><span class="sxs-lookup"><span data-stu-id="7b180-118">String</span></span> |  <span data-ttu-id="7b180-119">O segredo do cliente para autenticar a conexão com a instância do PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="7b180-119">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="7b180-120">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="7b180-120">**schoolsIds**</span></span> | <span data-ttu-id="7b180-121">String collection</span><span class="sxs-lookup"><span data-stu-id="7b180-121">String collection</span></span> |  <span data-ttu-id="7b180-122">A lista de escolas a ser sincronizada.</span><span class="sxs-lookup"><span data-stu-id="7b180-122">The list of schools to sync.</span></span> |
| <span data-ttu-id="7b180-123">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="7b180-123">**schoolYear**</span></span> | <span data-ttu-id="7b180-124">String</span><span class="sxs-lookup"><span data-stu-id="7b180-124">String</span></span> |  <span data-ttu-id="7b180-125">O ano escolar a ser sincronizado.</span><span class="sxs-lookup"><span data-stu-id="7b180-125">The school year to sync.</span></span> |
| <span data-ttu-id="7b180-126">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="7b180-126">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="7b180-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="7b180-127">Boolean</span></span> |  <span data-ttu-id="7b180-128">Indica se a fonte tem vários identificadores para um único aluno ou professor.</span><span class="sxs-lookup"><span data-stu-id="7b180-128">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="7b180-129">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="7b180-129">**customizations**</span></span> | [<span data-ttu-id="7b180-130">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="7b180-130">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="7b180-131">Personalização opcional a ser aplicada ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="7b180-131">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b180-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7b180-132">JSON representation</span></span>
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
