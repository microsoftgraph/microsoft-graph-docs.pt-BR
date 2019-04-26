---
title: tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e1dda51d5c98cb27ab9e71c7bef9167959c9052
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558234"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="7bfe3-103">tipo de recurso windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="7bfe3-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="7bfe3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bfe3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bfe3-106">Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-106">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="7bfe3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bfe3-107">Properties</span></span>
|<span data-ttu-id="7bfe3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bfe3-108">Property</span></span>|<span data-ttu-id="7bfe3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bfe3-109">Type</span></span>|<span data-ttu-id="7bfe3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bfe3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bfe3-111">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="7bfe3-111">applicableArchitecture</span></span>|[<span data-ttu-id="7bfe3-112">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="7bfe3-112">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="7bfe3-113">A arquitetura do Windows para a qual este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-113">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="7bfe3-114">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-114">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="7bfe3-115">displayName</span><span class="sxs-lookup"><span data-stu-id="7bfe3-115">displayName</span></span>|<span data-ttu-id="7bfe3-116">String</span><span class="sxs-lookup"><span data-stu-id="7bfe3-116">String</span></span>|<span data-ttu-id="7bfe3-117">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-117">The Display Name.</span></span>|
|<span data-ttu-id="7bfe3-118">identityName</span><span class="sxs-lookup"><span data-stu-id="7bfe3-118">identityName</span></span>|<span data-ttu-id="7bfe3-119">String</span><span class="sxs-lookup"><span data-stu-id="7bfe3-119">String</span></span>|<span data-ttu-id="7bfe3-120">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-120">The Identity Name.</span></span>|
|<span data-ttu-id="7bfe3-121">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="7bfe3-121">identityPublisher</span></span>|<span data-ttu-id="7bfe3-122">String</span><span class="sxs-lookup"><span data-stu-id="7bfe3-122">String</span></span>|<span data-ttu-id="7bfe3-123">O editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-123">The Identity Publisher.</span></span>|
|<span data-ttu-id="7bfe3-124">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7bfe3-124">identityResourceIdentifier</span></span>|<span data-ttu-id="7bfe3-125">String</span><span class="sxs-lookup"><span data-stu-id="7bfe3-125">String</span></span>|<span data-ttu-id="7bfe3-126">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-126">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="7bfe3-127">identityVersion</span><span class="sxs-lookup"><span data-stu-id="7bfe3-127">identityVersion</span></span>|<span data-ttu-id="7bfe3-128">String</span><span class="sxs-lookup"><span data-stu-id="7bfe3-128">String</span></span>|<span data-ttu-id="7bfe3-129">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-129">The Identity Version.</span></span>|
|<span data-ttu-id="7bfe3-130">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7bfe3-130">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="7bfe3-131">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="7bfe3-131">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="7bfe3-132">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-132">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bfe3-133">Relações</span><span class="sxs-lookup"><span data-stu-id="7bfe3-133">Relationships</span></span>
<span data-ttu-id="7bfe3-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7bfe3-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bfe3-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bfe3-135">JSON Representation</span></span>
<span data-ttu-id="7bfe3-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bfe3-136">Here is a JSON representation of the resource.</span></span>
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





