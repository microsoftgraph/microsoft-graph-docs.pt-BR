---
title: tipo de recurso mobileAppIntentAndStateDetail
description: Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 98b651168c9cb95e0672398ecad5b572be29de9e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42764597"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="0e214-103">tipo de recurso mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="0e214-103">mobileAppIntentAndStateDetail resource type</span></span>

> <span data-ttu-id="0e214-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e214-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e214-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e214-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e214-106">Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="0e214-106">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="0e214-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e214-107">Properties</span></span>
|<span data-ttu-id="0e214-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e214-108">Property</span></span>|<span data-ttu-id="0e214-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e214-109">Type</span></span>|<span data-ttu-id="0e214-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e214-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e214-111">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="0e214-111">applicationId</span></span>|<span data-ttu-id="0e214-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0e214-112">String</span></span>|<span data-ttu-id="0e214-113">Identificador MobieApp.</span><span class="sxs-lookup"><span data-stu-id="0e214-113">MobieApp identifier.</span></span>|
|<span data-ttu-id="0e214-114">displayName</span><span class="sxs-lookup"><span data-stu-id="0e214-114">displayName</span></span>|<span data-ttu-id="0e214-115">String</span><span class="sxs-lookup"><span data-stu-id="0e214-115">String</span></span>|<span data-ttu-id="0e214-116">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="0e214-116">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="0e214-117">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="0e214-117">mobileAppIntent</span></span>|[<span data-ttu-id="0e214-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="0e214-118">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="0e214-119">Tentativa de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="0e214-119">Mobile App Intent.</span></span> <span data-ttu-id="0e214-120">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="0e214-120">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="0e214-121">displayVersion</span><span class="sxs-lookup"><span data-stu-id="0e214-121">displayVersion</span></span>|<span data-ttu-id="0e214-122">String</span><span class="sxs-lookup"><span data-stu-id="0e214-122">String</span></span>|<span data-ttu-id="0e214-123">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="0e214-123">Human readable version of the application</span></span>|
|<span data-ttu-id="0e214-124">installState</span><span class="sxs-lookup"><span data-stu-id="0e214-124">installState</span></span>|[<span data-ttu-id="0e214-125">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="0e214-125">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="0e214-126">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0e214-126">The install state of the app.</span></span> <span data-ttu-id="0e214-127">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="0e214-127">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="0e214-128">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="0e214-128">supportedDeviceTypes</span></span>|<span data-ttu-id="0e214-129">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="0e214-129">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="0e214-130">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0e214-130">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e214-131">Relações</span><span class="sxs-lookup"><span data-stu-id="0e214-131">Relationships</span></span>
<span data-ttu-id="0e214-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e214-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e214-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e214-133">JSON Representation</span></span>
<span data-ttu-id="0e214-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e214-134">Here is a JSON representation of the resource.</span></span>
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



