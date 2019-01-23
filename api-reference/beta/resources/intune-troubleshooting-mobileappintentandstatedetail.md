---
title: tipo de recurso de mobileAppIntentAndStateDetail
description: A intenção de App Mobile e o estado de instalação para um determinado dispositivo.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ef88a1fa346784ae00a125a487ca844c58d62eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414253"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="766af-103">tipo de recurso de mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="766af-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="766af-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="766af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="766af-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="766af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="766af-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="766af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="766af-107">A intenção de App Mobile e o estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="766af-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="766af-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="766af-108">Properties</span></span>
|<span data-ttu-id="766af-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="766af-109">Property</span></span>|<span data-ttu-id="766af-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="766af-110">Type</span></span>|<span data-ttu-id="766af-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="766af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="766af-112">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="766af-112">applicationId</span></span>|<span data-ttu-id="766af-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="766af-113">String</span></span>|<span data-ttu-id="766af-114">Identificador de MobieApp.</span><span class="sxs-lookup"><span data-stu-id="766af-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="766af-115">displayName</span><span class="sxs-lookup"><span data-stu-id="766af-115">displayName</span></span>|<span data-ttu-id="766af-116">String</span><span class="sxs-lookup"><span data-stu-id="766af-116">String</span></span>|<span data-ttu-id="766af-117">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="766af-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="766af-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="766af-118">mobileAppIntent</span></span>|[<span data-ttu-id="766af-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="766af-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="766af-120">Intenção de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="766af-120">Mobile App Intent.</span></span> <span data-ttu-id="766af-121">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="766af-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="766af-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="766af-122">displayVersion</span></span>|<span data-ttu-id="766af-123">String</span><span class="sxs-lookup"><span data-stu-id="766af-123">String</span></span>|<span data-ttu-id="766af-124">Versão legível humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="766af-124">Human readable version of the application</span></span>|
|<span data-ttu-id="766af-125">installState</span><span class="sxs-lookup"><span data-stu-id="766af-125">installState</span></span>|[<span data-ttu-id="766af-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="766af-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="766af-127">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="766af-127">The install state of the app.</span></span> <span data-ttu-id="766af-128">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="766af-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="766af-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="766af-129">supportedDeviceTypes</span></span>|<span data-ttu-id="766af-130">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="766af-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="766af-131">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="766af-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="766af-132">Relações</span><span class="sxs-lookup"><span data-stu-id="766af-132">Relationships</span></span>
<span data-ttu-id="766af-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="766af-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="766af-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="766af-134">JSON Representation</span></span>
<span data-ttu-id="766af-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="766af-135">Here is a JSON representation of the resource.</span></span>
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




