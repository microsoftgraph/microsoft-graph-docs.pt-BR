---
title: tipo de recurso de windowsPackageInformation
description: Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac0f9aad1cdba1eaaac12754fd4a4d0ad4a6db32
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27926845"
---
# <a name="windowspackageinformation-resource-type"></a><span data-ttu-id="f5f2a-103">tipo de recurso de windowsPackageInformation</span><span class="sxs-lookup"><span data-stu-id="f5f2a-103">windowsPackageInformation resource type</span></span>

> <span data-ttu-id="f5f2a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5f2a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f5f2a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5f2a-107">Contém propriedades para as informações de pacote para uma linha do Windows do aplicativo de negócios.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-107">Contains properties for the package information for a Windows line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="f5f2a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5f2a-108">Properties</span></span>
|<span data-ttu-id="f5f2a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5f2a-109">Property</span></span>|<span data-ttu-id="f5f2a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5f2a-110">Type</span></span>|<span data-ttu-id="f5f2a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5f2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5f2a-112">applicableArchitecture</span><span class="sxs-lookup"><span data-stu-id="f5f2a-112">applicableArchitecture</span></span>|[<span data-ttu-id="f5f2a-113">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="f5f2a-113">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="f5f2a-114">A arquitetura do Windows para a qual este aplicativo pode executar em.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-114">The Windows architecture for which this app can run on.</span></span> <span data-ttu-id="f5f2a-115">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-115">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="f5f2a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f5f2a-116">displayName</span></span>|<span data-ttu-id="f5f2a-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5f2a-117">String</span></span>|<span data-ttu-id="f5f2a-118">O nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-118">The Display Name.</span></span>|
|<span data-ttu-id="f5f2a-119">identityName</span><span class="sxs-lookup"><span data-stu-id="f5f2a-119">identityName</span></span>|<span data-ttu-id="f5f2a-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5f2a-120">String</span></span>|<span data-ttu-id="f5f2a-121">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-121">The Identity Name.</span></span>|
|<span data-ttu-id="f5f2a-122">identityPublisher</span><span class="sxs-lookup"><span data-stu-id="f5f2a-122">identityPublisher</span></span>|<span data-ttu-id="f5f2a-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5f2a-123">String</span></span>|<span data-ttu-id="f5f2a-124">O Editor de identidade.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-124">The Identity Publisher.</span></span>|
|<span data-ttu-id="f5f2a-125">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f5f2a-125">identityResourceIdentifier</span></span>|<span data-ttu-id="f5f2a-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5f2a-126">String</span></span>|<span data-ttu-id="f5f2a-127">O Identificador de Recurso da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-127">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="f5f2a-128">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f5f2a-128">identityVersion</span></span>|<span data-ttu-id="f5f2a-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f5f2a-129">String</span></span>|<span data-ttu-id="f5f2a-130">A versão de identidade.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-130">The Identity Version.</span></span>|
|<span data-ttu-id="f5f2a-131">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f5f2a-131">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f5f2a-132">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f5f2a-132">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f5f2a-133">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-133">The value for the minimum applicable operating system.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f5f2a-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f5f2a-134">Relationships</span></span>
<span data-ttu-id="f5f2a-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5f2a-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f5f2a-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5f2a-136">JSON Representation</span></span>
<span data-ttu-id="f5f2a-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5f2a-137">Here is a JSON representation of the resource.</span></span>
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





