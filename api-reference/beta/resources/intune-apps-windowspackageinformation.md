---
title: tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a35500a2895ad697ec7881e52d6db83f19871b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012167"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="222c7-103">tipo de recurso windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="222c7-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="222c7-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="222c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="222c7-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="222c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="222c7-106">Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.</span><span class="sxs-lookup"><span data-stu-id="222c7-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="222c7-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="222c7-107">Properties</span></span>
|<span data-ttu-id="222c7-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="222c7-108">Property</span></span>|<span data-ttu-id="222c7-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="222c7-109">Type</span></span>|<span data-ttu-id="222c7-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="222c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="222c7-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="222c7-111">applicableArchitecture</span></span>|[<span data-ttu-id="222c7-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="222c7-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="222c7-113">A arquitetura do Windows para a qual este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="222c7-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="222c7-114">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="222c7-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="222c7-115">displayName</span><span class="sxs-lookup"><span data-stu-id="222c7-115">displayName</span></span>|<span data-ttu-id="222c7-116">String</span><span class="sxs-lookup"><span data-stu-id="222c7-116">String</span></span>|<span data-ttu-id="222c7-117">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="222c7-117">The Display Name.</span></span>|
|<span data-ttu-id="222c7-118">identityName</span><span class="sxs-lookup"><span data-stu-id="222c7-118">identityName</span></span>|<span data-ttu-id="222c7-119">String</span><span class="sxs-lookup"><span data-stu-id="222c7-119">String</span></span>|<span data-ttu-id="222c7-120">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="222c7-120">The Identity Name.</span></span>|
|<span data-ttu-id="222c7-121">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="222c7-121">identityPublisher</span></span>|<span data-ttu-id="222c7-122">String</span><span class="sxs-lookup"><span data-stu-id="222c7-122">String</span></span>|<span data-ttu-id="222c7-123">O editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="222c7-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="222c7-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="222c7-124">identityResourceIdentifier</span></span>|<span data-ttu-id="222c7-125">String</span><span class="sxs-lookup"><span data-stu-id="222c7-125">String</span></span>|<span data-ttu-id="222c7-126">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="222c7-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="222c7-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="222c7-127">identityVersion</span></span>|<span data-ttu-id="222c7-128">String</span><span class="sxs-lookup"><span data-stu-id="222c7-128">String</span></span>|<span data-ttu-id="222c7-129">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="222c7-129">The Identity Version.</span></span>|
|<span data-ttu-id="222c7-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="222c7-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="222c7-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="222c7-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="222c7-132">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="222c7-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="222c7-133">Relações</span><span class="sxs-lookup"><span data-stu-id="222c7-133">Relationships</span></span>
<span data-ttu-id="222c7-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="222c7-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="222c7-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="222c7-135">JSON Representation</span></span>
<span data-ttu-id="222c7-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="222c7-136">Here is a JSON representation of the resource.</span></span>
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





