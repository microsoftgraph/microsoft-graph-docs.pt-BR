---
title: tipo de recurso de mobileAppIntentAndStateDetail
description: A intenção de App Mobile e o estado de instalação para um determinado dispositivo.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad20ef00cbc8e5295a96107fbce2f5e7f1cb978a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805807"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="8510e-103">tipo de recurso de mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="8510e-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="8510e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8510e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8510e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8510e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8510e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8510e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8510e-107">A intenção de App Mobile e o estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8510e-107">Mobile App Intent and Install State for a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="8510e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8510e-108">Properties</span></span>
|<span data-ttu-id="8510e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8510e-109">Property</span></span>|<span data-ttu-id="8510e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8510e-110">Type</span></span>|<span data-ttu-id="8510e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8510e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8510e-112">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="8510e-112">applicationId</span></span>|<span data-ttu-id="8510e-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8510e-113">String</span></span>|<span data-ttu-id="8510e-114">Identificador de MobieApp.</span><span class="sxs-lookup"><span data-stu-id="8510e-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="8510e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="8510e-115">displayName</span></span>|<span data-ttu-id="8510e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8510e-116">String</span></span>|<span data-ttu-id="8510e-117">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="8510e-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="8510e-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="8510e-118">mobileAppIntent</span></span>|[<span data-ttu-id="8510e-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="8510e-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="8510e-120">Intenção de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="8510e-120">Mobile App Intent.</span></span> <span data-ttu-id="8510e-121">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="8510e-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="8510e-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="8510e-122">displayVersion</span></span>|<span data-ttu-id="8510e-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8510e-123">String</span></span>|<span data-ttu-id="8510e-124">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="8510e-124">Human readable version of the application</span></span>|
|<span data-ttu-id="8510e-125">installState</span><span class="sxs-lookup"><span data-stu-id="8510e-125">installState</span></span>|[<span data-ttu-id="8510e-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="8510e-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="8510e-127">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8510e-127">The install state of the app.</span></span> <span data-ttu-id="8510e-128">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="8510e-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="8510e-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="8510e-129">supportedDeviceTypes</span></span>|<span data-ttu-id="8510e-130">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="8510e-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="8510e-131">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8510e-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8510e-132">Relações</span><span class="sxs-lookup"><span data-stu-id="8510e-132">Relationships</span></span>
<span data-ttu-id="8510e-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8510e-133">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8510e-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8510e-134">JSON Representation</span></span>
<span data-ttu-id="8510e-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8510e-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppIntentAndStateDetail",
  "applicationId": "String",
  "displayName": "String",
  "mobileAppIntent": "String",
  "displayVersion": "String",
  "installState": "String",
  "supportedDeviceTypes": [
    {
      "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
      "type": "String",
      "minimumOperatingSystemVersion": "String",
      "maximumOperatingSystemVersion": "String"
    }
  ]
}
```





