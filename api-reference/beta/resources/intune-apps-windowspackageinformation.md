---
title: tipo de recurso de windowsPackageInformation
description: Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 112d84c5bae889e24b889b4598d61a6b3d63db50
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403277"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="9bbac-103">tipo de recurso de windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="9bbac-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="9bbac-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9bbac-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9bbac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9bbac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bbac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9bbac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9bbac-107">Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.</span><span class="sxs-lookup"><span data-stu-id="9bbac-107">Contains properties for the package information for a Windows line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="9bbac-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9bbac-108">Properties</span></span>
|<span data-ttu-id="9bbac-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9bbac-109">Property</span></span>|<span data-ttu-id="9bbac-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9bbac-110">Type</span></span>|<span data-ttu-id="9bbac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9bbac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bbac-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="9bbac-112">applicableArchitecture</span></span>|[<span data-ttu-id="9bbac-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="9bbac-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="9bbac-114">A arquitetura do Windows para a qual este aplicativo pode executar em.</span><span class="sxs-lookup"><span data-stu-id="9bbac-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="9bbac-115">Os possíveis valores são: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span><span class="sxs-lookup"><span data-stu-id="9bbac-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="9bbac-116">displayName</span><span class="sxs-lookup"><span data-stu-id="9bbac-116">displayName</span></span>|<span data-ttu-id="9bbac-117">String</span><span class="sxs-lookup"><span data-stu-id="9bbac-117">String</span></span>|<span data-ttu-id="9bbac-118">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9bbac-118">The Display Name.</span></span>|
|<span data-ttu-id="9bbac-119">identityName</span><span class="sxs-lookup"><span data-stu-id="9bbac-119">identityName</span></span>|<span data-ttu-id="9bbac-120">String</span><span class="sxs-lookup"><span data-stu-id="9bbac-120">String</span></span>|<span data-ttu-id="9bbac-121">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9bbac-121">The Identity Name.</span></span>|
|<span data-ttu-id="9bbac-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="9bbac-122">identityPublisher</span></span>|<span data-ttu-id="9bbac-123">String</span><span class="sxs-lookup"><span data-stu-id="9bbac-123">String</span></span>|<span data-ttu-id="9bbac-124">O Editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="9bbac-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="9bbac-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="9bbac-125">identityResourceIdentifier</span></span>|<span data-ttu-id="9bbac-126">String</span><span class="sxs-lookup"><span data-stu-id="9bbac-126">String</span></span>|<span data-ttu-id="9bbac-127">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="9bbac-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="9bbac-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="9bbac-128">identityVersion</span></span>|<span data-ttu-id="9bbac-129">String</span><span class="sxs-lookup"><span data-stu-id="9bbac-129">String</span></span>|<span data-ttu-id="9bbac-130">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="9bbac-130">The Identity Version.</span></span>|
|<span data-ttu-id="9bbac-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9bbac-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="9bbac-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="9bbac-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="9bbac-133">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="9bbac-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9bbac-134">Relações</span><span class="sxs-lookup"><span data-stu-id="9bbac-134">Relationships</span></span>
<span data-ttu-id="9bbac-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9bbac-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bbac-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9bbac-136">JSON Representation</span></span>
<span data-ttu-id="9bbac-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9bbac-137">Here is a JSON representation of the resource.</span></span>
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




