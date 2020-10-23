---
title: tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9a7871a101062e9d835c68f37299d83a8bfb5e8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726553"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="b151d-103">tipo de recurso windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="b151d-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="b151d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b151d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b151d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b151d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b151d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b151d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b151d-107">Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.</span><span class="sxs-lookup"><span data-stu-id="b151d-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="b151d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b151d-108">Properties</span></span>
|<span data-ttu-id="b151d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b151d-109">Property</span></span>|<span data-ttu-id="b151d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b151d-110">Type</span></span>|<span data-ttu-id="b151d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b151d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b151d-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="b151d-112">applicableArchitecture</span></span>|[<span data-ttu-id="b151d-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b151d-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b151d-114">A arquitetura do Windows para a qual este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="b151d-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="b151d-115">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="b151d-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b151d-116">displayName</span><span class="sxs-lookup"><span data-stu-id="b151d-116">displayName</span></span>|<span data-ttu-id="b151d-117">String</span><span class="sxs-lookup"><span data-stu-id="b151d-117">String</span></span>|<span data-ttu-id="b151d-118">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b151d-118">The Display Name.</span></span>|
|<span data-ttu-id="b151d-119">identityName</span><span class="sxs-lookup"><span data-stu-id="b151d-119">identityName</span></span>|<span data-ttu-id="b151d-120">String</span><span class="sxs-lookup"><span data-stu-id="b151d-120">String</span></span>|<span data-ttu-id="b151d-121">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b151d-121">The Identity Name.</span></span>|
|<span data-ttu-id="b151d-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="b151d-122">identityPublisher</span></span>|<span data-ttu-id="b151d-123">String</span><span class="sxs-lookup"><span data-stu-id="b151d-123">String</span></span>|<span data-ttu-id="b151d-124">O editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="b151d-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="b151d-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b151d-125">identityResourceIdentifier</span></span>|<span data-ttu-id="b151d-126">String</span><span class="sxs-lookup"><span data-stu-id="b151d-126">String</span></span>|<span data-ttu-id="b151d-127">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="b151d-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="b151d-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="b151d-128">identityVersion</span></span>|<span data-ttu-id="b151d-129">String</span><span class="sxs-lookup"><span data-stu-id="b151d-129">String</span></span>|<span data-ttu-id="b151d-130">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="b151d-130">The Identity Version.</span></span>|
|<span data-ttu-id="b151d-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b151d-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b151d-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b151d-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="b151d-133">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="b151d-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b151d-134">Relações</span><span class="sxs-lookup"><span data-stu-id="b151d-134">Relationships</span></span>
<span data-ttu-id="b151d-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b151d-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b151d-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b151d-136">JSON Representation</span></span>
<span data-ttu-id="b151d-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b151d-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true,
    "v10_1809": true,
    "v10_1903": true
  }
}
```





