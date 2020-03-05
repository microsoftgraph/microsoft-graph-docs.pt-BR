---
title: tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e3b0f79614726b74ca2af3662689dc46b7c2df25
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489815"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="1057a-103">tipo de recurso windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="1057a-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="1057a-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1057a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1057a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1057a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1057a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1057a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1057a-107">Contém propriedades para as informações de pacote de um aplicativo de linha de negócios do Windows.</span><span class="sxs-lookup"><span data-stu-id="1057a-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="1057a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1057a-108">Properties</span></span>
|<span data-ttu-id="1057a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1057a-109">Property</span></span>|<span data-ttu-id="1057a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1057a-110">Type</span></span>|<span data-ttu-id="1057a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1057a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1057a-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="1057a-112">applicableArchitecture</span></span>|[<span data-ttu-id="1057a-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1057a-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1057a-114">A arquitetura do Windows para a qual este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1057a-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="1057a-115">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="1057a-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="1057a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1057a-116">displayName</span></span>|<span data-ttu-id="1057a-117">String</span><span class="sxs-lookup"><span data-stu-id="1057a-117">String</span></span>|<span data-ttu-id="1057a-118">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1057a-118">The Display Name.</span></span>|
|<span data-ttu-id="1057a-119">identityName</span><span class="sxs-lookup"><span data-stu-id="1057a-119">identityName</span></span>|<span data-ttu-id="1057a-120">String</span><span class="sxs-lookup"><span data-stu-id="1057a-120">String</span></span>|<span data-ttu-id="1057a-121">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1057a-121">The Identity Name.</span></span>|
|<span data-ttu-id="1057a-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="1057a-122">identityPublisher</span></span>|<span data-ttu-id="1057a-123">String</span><span class="sxs-lookup"><span data-stu-id="1057a-123">String</span></span>|<span data-ttu-id="1057a-124">O editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="1057a-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="1057a-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1057a-125">identityResourceIdentifier</span></span>|<span data-ttu-id="1057a-126">String</span><span class="sxs-lookup"><span data-stu-id="1057a-126">String</span></span>|<span data-ttu-id="1057a-127">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1057a-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="1057a-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1057a-128">identityVersion</span></span>|<span data-ttu-id="1057a-129">String</span><span class="sxs-lookup"><span data-stu-id="1057a-129">String</span></span>|<span data-ttu-id="1057a-130">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="1057a-130">The Identity Version.</span></span>|
|<span data-ttu-id="1057a-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1057a-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1057a-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1057a-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1057a-133">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1057a-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1057a-134">Relações</span><span class="sxs-lookup"><span data-stu-id="1057a-134">Relationships</span></span>
<span data-ttu-id="1057a-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1057a-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1057a-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1057a-136">JSON Representation</span></span>
<span data-ttu-id="1057a-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1057a-137">Here is a JSON representation of the resource.</span></span>
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



