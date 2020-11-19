---
title: tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 409d9aedf0ef42114269b1d1d23e9fd5d08e8faa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49284271"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="613a3-103">tipo de recurso windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="613a3-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="613a3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="613a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="613a3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="613a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="613a3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="613a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="613a3-107">Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.</span><span class="sxs-lookup"><span data-stu-id="613a3-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="613a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="613a3-108">Properties</span></span>
|<span data-ttu-id="613a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="613a3-109">Property</span></span>|<span data-ttu-id="613a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="613a3-110">Type</span></span>|<span data-ttu-id="613a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="613a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="613a3-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="613a3-112">applicableArchitecture</span></span>|[<span data-ttu-id="613a3-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="613a3-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="613a3-114">A arquitetura do Windows para a qual este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="613a3-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="613a3-115">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="613a3-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="613a3-116">displayName</span><span class="sxs-lookup"><span data-stu-id="613a3-116">displayName</span></span>|<span data-ttu-id="613a3-117">String</span><span class="sxs-lookup"><span data-stu-id="613a3-117">String</span></span>|<span data-ttu-id="613a3-118">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="613a3-118">The Display Name.</span></span>|
|<span data-ttu-id="613a3-119">identityName</span><span class="sxs-lookup"><span data-stu-id="613a3-119">identityName</span></span>|<span data-ttu-id="613a3-120">String</span><span class="sxs-lookup"><span data-stu-id="613a3-120">String</span></span>|<span data-ttu-id="613a3-121">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="613a3-121">The Identity Name.</span></span>|
|<span data-ttu-id="613a3-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="613a3-122">identityPublisher</span></span>|<span data-ttu-id="613a3-123">String</span><span class="sxs-lookup"><span data-stu-id="613a3-123">String</span></span>|<span data-ttu-id="613a3-124">O editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="613a3-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="613a3-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="613a3-125">identityResourceIdentifier</span></span>|<span data-ttu-id="613a3-126">String</span><span class="sxs-lookup"><span data-stu-id="613a3-126">String</span></span>|<span data-ttu-id="613a3-127">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="613a3-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="613a3-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="613a3-128">identityVersion</span></span>|<span data-ttu-id="613a3-129">String</span><span class="sxs-lookup"><span data-stu-id="613a3-129">String</span></span>|<span data-ttu-id="613a3-130">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="613a3-130">The Identity Version.</span></span>|
|<span data-ttu-id="613a3-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="613a3-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="613a3-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="613a3-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="613a3-133">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="613a3-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="613a3-134">Relações</span><span class="sxs-lookup"><span data-stu-id="613a3-134">Relationships</span></span>
<span data-ttu-id="613a3-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="613a3-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="613a3-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="613a3-136">JSON Representation</span></span>
<span data-ttu-id="613a3-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="613a3-137">Here is a JSON representation of the resource.</span></span>
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




