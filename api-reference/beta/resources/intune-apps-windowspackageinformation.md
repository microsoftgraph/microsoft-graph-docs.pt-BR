---
title: Tipo de recurso windowsPackageInformation
description: Contém propriedades para as informações do pacote para um aplicativo de linha de negócios do Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b2474fe5458c7a8c8fcc54d354f46ec7386952e
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866304"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="1e86e-103">Tipo de recurso windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="1e86e-103">windowsPackageInformation resource type</span></span>

<span data-ttu-id="1e86e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e86e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e86e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1e86e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e86e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e86e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e86e-107">Contém propriedades para as informações do pacote para um aplicativo de linha de negócios do Windows.</span><span class="sxs-lookup"><span data-stu-id="1e86e-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="1e86e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1e86e-108">Properties</span></span>
|<span data-ttu-id="1e86e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e86e-109">Property</span></span>|<span data-ttu-id="1e86e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e86e-110">Type</span></span>|<span data-ttu-id="1e86e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e86e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e86e-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="1e86e-112">applicableArchitecture</span></span>|[<span data-ttu-id="1e86e-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1e86e-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1e86e-114">A arquitetura do Windows na qual este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="1e86e-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="1e86e-115">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="1e86e-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="1e86e-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1e86e-116">displayName</span></span>|<span data-ttu-id="1e86e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1e86e-117">String</span></span>|<span data-ttu-id="1e86e-118">O Nome para Exibição.</span><span class="sxs-lookup"><span data-stu-id="1e86e-118">The Display Name.</span></span>|
|<span data-ttu-id="1e86e-119">identityName</span><span class="sxs-lookup"><span data-stu-id="1e86e-119">identityName</span></span>|<span data-ttu-id="1e86e-120">String</span><span class="sxs-lookup"><span data-stu-id="1e86e-120">String</span></span>|<span data-ttu-id="1e86e-121">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1e86e-121">The Identity Name.</span></span>|
|<span data-ttu-id="1e86e-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="1e86e-122">identityPublisher</span></span>|<span data-ttu-id="1e86e-123">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1e86e-123">String</span></span>|<span data-ttu-id="1e86e-124">O Editor de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1e86e-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="1e86e-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1e86e-125">identityResourceIdentifier</span></span>|<span data-ttu-id="1e86e-126">String</span><span class="sxs-lookup"><span data-stu-id="1e86e-126">String</span></span>|<span data-ttu-id="1e86e-127">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="1e86e-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="1e86e-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1e86e-128">identityVersion</span></span>|<span data-ttu-id="1e86e-129">String</span><span class="sxs-lookup"><span data-stu-id="1e86e-129">String</span></span>|<span data-ttu-id="1e86e-130">A Versão de Identidade.</span><span class="sxs-lookup"><span data-stu-id="1e86e-130">The Identity Version.</span></span>|
|<span data-ttu-id="1e86e-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e86e-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1e86e-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1e86e-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1e86e-133">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="1e86e-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e86e-134">Relações</span><span class="sxs-lookup"><span data-stu-id="1e86e-134">Relationships</span></span>
<span data-ttu-id="1e86e-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1e86e-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e86e-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1e86e-136">JSON Representation</span></span>
<span data-ttu-id="1e86e-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1e86e-137">Here is a JSON representation of the resource.</span></span>
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
    "v10_1903": true,
    "v10_1909": true,
    "v10_2004": true,
    "v10_2H20": true
  }
}
```




