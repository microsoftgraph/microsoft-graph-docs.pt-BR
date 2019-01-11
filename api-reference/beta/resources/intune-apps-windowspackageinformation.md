---
title: tipo de recurso de windowsPackageInformation
description: Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f7f3cd593670e071ae62bdb287bcebeee01d555
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849529"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="add90-103">tipo de recurso de windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="add90-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="add90-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="add90-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="add90-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="add90-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="add90-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="add90-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="add90-107">Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.</span><span class="sxs-lookup"><span data-stu-id="add90-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="add90-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="add90-108">Properties</span></span>
|<span data-ttu-id="add90-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="add90-109">Property</span></span>|<span data-ttu-id="add90-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="add90-110">Type</span></span>|<span data-ttu-id="add90-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="add90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="add90-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="add90-112">applicableArchitecture</span></span>|[<span data-ttu-id="add90-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="add90-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="add90-114">A arquitetura do Windows para a qual este aplicativo pode executar em.</span><span class="sxs-lookup"><span data-stu-id="add90-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="add90-115">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="add90-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="add90-116">displayName</span><span class="sxs-lookup"><span data-stu-id="add90-116">displayName</span></span>|<span data-ttu-id="add90-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="add90-117">String</span></span>|<span data-ttu-id="add90-118">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="add90-118">The Display Name.</span></span>|
|<span data-ttu-id="add90-119">identityName</span><span class="sxs-lookup"><span data-stu-id="add90-119">identityName</span></span>|<span data-ttu-id="add90-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="add90-120">String</span></span>|<span data-ttu-id="add90-121">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="add90-121">The Identity Name.</span></span>|
|<span data-ttu-id="add90-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="add90-122">identityPublisher</span></span>|<span data-ttu-id="add90-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="add90-123">String</span></span>|<span data-ttu-id="add90-124">O Editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="add90-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="add90-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="add90-125">identityResourceIdentifier</span></span>|<span data-ttu-id="add90-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="add90-126">String</span></span>|<span data-ttu-id="add90-127">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="add90-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="add90-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="add90-128">identityVersion</span></span>|<span data-ttu-id="add90-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="add90-129">String</span></span>|<span data-ttu-id="add90-130">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="add90-130">The Identity Version.</span></span>|
|<span data-ttu-id="add90-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="add90-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="add90-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="add90-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="add90-133">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="add90-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="add90-134">Relações</span><span class="sxs-lookup"><span data-stu-id="add90-134">Relationships</span></span>
<span data-ttu-id="add90-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="add90-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="add90-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="add90-136">JSON Representation</span></span>
<span data-ttu-id="add90-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="add90-137">Here is a JSON representation of the resource.</span></span>
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





