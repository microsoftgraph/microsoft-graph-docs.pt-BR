---
title: recurso de educationPowerSchoolDataProvider
description: Usado para configurar o perfil de sincronização de dados da escola quando PowerSchool é usado como a fonte de entrada.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4028170c2780cee426ec961a44b51e0362b0187f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406917"
---
# <a name="educationpowerschooldataprovider-resource"></a><span data-ttu-id="735df-103">recurso de educationPowerSchoolDataProvider</span><span class="sxs-lookup"><span data-stu-id="735df-103">educationPowerSchoolDataProvider resource</span></span>

> <span data-ttu-id="735df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="735df-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="735df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="735df-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="735df-106">Usado para configurar o perfil de sincronização de dados da escola quando [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) é usado como a fonte de entrada.</span><span class="sxs-lookup"><span data-stu-id="735df-106">Used to set up the school data synchronization profile when [PowerSchool](https://www.powerschool.com/solutions/student-information-system-sis/) is used as the input source.</span></span>

<span data-ttu-id="735df-107">Derivado do [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span><span class="sxs-lookup"><span data-stu-id="735df-107">Derived from [educationSynchronizationDataProvider](educationsynchronizationdataprovider.md).</span></span>

## <a name="properties"></a><span data-ttu-id="735df-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="735df-108">Properties</span></span>

| <span data-ttu-id="735df-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="735df-109">Property</span></span> | <span data-ttu-id="735df-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="735df-110">Type</span></span> | <span data-ttu-id="735df-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="735df-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="735df-112">**URL de conexão**</span><span class="sxs-lookup"><span data-stu-id="735df-112">**connectionUrl**</span></span> | <span data-ttu-id="735df-113">String</span><span class="sxs-lookup"><span data-stu-id="735df-113">String</span></span> | <span data-ttu-id="735df-114">A URL da conexão para a instância de PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="735df-114">The connection URL to the PowerSchool instance.</span></span> |
| <span data-ttu-id="735df-115">**clientId**</span><span class="sxs-lookup"><span data-stu-id="735df-115">**clientId**</span></span> | <span data-ttu-id="735df-116">String</span><span class="sxs-lookup"><span data-stu-id="735df-116">String</span></span> |  <span data-ttu-id="735df-117">A identificação do cliente usada para conectar ao PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="735df-117">The client ID used to connect to PowerSchool.</span></span> |
| <span data-ttu-id="735df-118">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="735df-118">**clientSecret**</span></span> | <span data-ttu-id="735df-119">String</span><span class="sxs-lookup"><span data-stu-id="735df-119">String</span></span> |  <span data-ttu-id="735df-120">O segredo do cliente para autenticar a conexão à instância PowerSchool.</span><span class="sxs-lookup"><span data-stu-id="735df-120">The client secret to authenticate the connection to the PowerSchool instance.</span></span> |
| <span data-ttu-id="735df-121">**schoolsIds**</span><span class="sxs-lookup"><span data-stu-id="735df-121">**schoolsIds**</span></span> | <span data-ttu-id="735df-122">String collection</span><span class="sxs-lookup"><span data-stu-id="735df-122">String collection</span></span> |  <span data-ttu-id="735df-123">A lista de escolas para sincronizar.</span><span class="sxs-lookup"><span data-stu-id="735df-123">The list of schools to sync.</span></span> |
| <span data-ttu-id="735df-124">**schoolYear**</span><span class="sxs-lookup"><span data-stu-id="735df-124">**schoolYear**</span></span> | <span data-ttu-id="735df-125">String</span><span class="sxs-lookup"><span data-stu-id="735df-125">String</span></span> |  <span data-ttu-id="735df-126">O ano escola para sincronizar.</span><span class="sxs-lookup"><span data-stu-id="735df-126">The school year to sync.</span></span> |
| <span data-ttu-id="735df-127">**allowTeachersInMultipleSchools**</span><span class="sxs-lookup"><span data-stu-id="735df-127">**allowTeachersInMultipleSchools**</span></span> | <span data-ttu-id="735df-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="735df-128">Boolean</span></span> |  <span data-ttu-id="735df-129">Indica se a fonte tem vários identificadores para um único aluno ou professor.</span><span class="sxs-lookup"><span data-stu-id="735df-129">Indicates whether the source has multiple identifiers for a single student or teacher.</span></span> |
| <span data-ttu-id="735df-130">**personalizações**</span><span class="sxs-lookup"><span data-stu-id="735df-130">**customizations**</span></span> | [<span data-ttu-id="735df-131">educationSynchronizationCustomizations</span><span class="sxs-lookup"><span data-stu-id="735df-131">educationSynchronizationCustomizations</span></span>](educationsynchronizationcustomizations.md) | <span data-ttu-id="735df-132">Personalização opcional a ser aplicado ao perfil de sincronização.</span><span class="sxs-lookup"><span data-stu-id="735df-132">Optional customization to be applied to the synchronization profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="735df-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="735df-133">JSON representation</span></span>
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
