---
title: tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2803779830d0e2bb88a0a91a96abfc101d15cb66
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949497"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="2ecf8-103">tipo de recurso windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="2ecf8-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="2ecf8-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ecf8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ecf8-106">Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="2ecf8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2ecf8-107">Properties</span></span>
|<span data-ttu-id="2ecf8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2ecf8-108">Property</span></span>|<span data-ttu-id="2ecf8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="2ecf8-109">Type</span></span>|<span data-ttu-id="2ecf8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2ecf8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ecf8-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="2ecf8-111">applicableArchitecture</span></span>|[<span data-ttu-id="2ecf8-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="2ecf8-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="2ecf8-113">A arquitetura do Windows para a qual este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="2ecf8-114">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="2ecf8-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2ecf8-115">displayName</span></span>|<span data-ttu-id="2ecf8-116">String</span><span class="sxs-lookup"><span data-stu-id="2ecf8-116">String</span></span>|<span data-ttu-id="2ecf8-117">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-117">The Display Name.</span></span>|
|<span data-ttu-id="2ecf8-118">identityName</span><span class="sxs-lookup"><span data-stu-id="2ecf8-118">identityName</span></span>|<span data-ttu-id="2ecf8-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ecf8-119">String</span></span>|<span data-ttu-id="2ecf8-120">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-120">The Identity Name.</span></span>|
|<span data-ttu-id="2ecf8-121">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="2ecf8-121">identityPublisher</span></span>|<span data-ttu-id="2ecf8-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2ecf8-122">String</span></span>|<span data-ttu-id="2ecf8-123">O editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="2ecf8-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ecf8-124">identityResourceIdentifier</span></span>|<span data-ttu-id="2ecf8-125">String</span><span class="sxs-lookup"><span data-stu-id="2ecf8-125">String</span></span>|<span data-ttu-id="2ecf8-126">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="2ecf8-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2ecf8-127">identityVersion</span></span>|<span data-ttu-id="2ecf8-128">String</span><span class="sxs-lookup"><span data-stu-id="2ecf8-128">String</span></span>|<span data-ttu-id="2ecf8-129">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-129">The Identity Version.</span></span>|
|<span data-ttu-id="2ecf8-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ecf8-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2ecf8-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2ecf8-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2ecf8-132">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ecf8-133">Relações</span><span class="sxs-lookup"><span data-stu-id="2ecf8-133">Relationships</span></span>
<span data-ttu-id="2ecf8-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2ecf8-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ecf8-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2ecf8-135">JSON Representation</span></span>
<span data-ttu-id="2ecf8-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2ecf8-136">Here is a JSON representation of the resource.</span></span>
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
    "v10_1803": true
  }
}
```




