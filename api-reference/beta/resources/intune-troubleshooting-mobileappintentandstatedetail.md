---
title: tipo de recurso mobileAppIntentAndStateDetail
description: Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2fa57fb4218d961d8d3e58eb284062998903325b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003588"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="18572-103">tipo de recurso mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="18572-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="18572-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="18572-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18572-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="18572-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18572-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18572-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18572-107">Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="18572-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="18572-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18572-108">Properties</span></span>
|<span data-ttu-id="18572-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18572-109">Property</span></span>|<span data-ttu-id="18572-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="18572-110">Type</span></span>|<span data-ttu-id="18572-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18572-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18572-112">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="18572-112">applicationId</span></span>|<span data-ttu-id="18572-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="18572-113">String</span></span>|<span data-ttu-id="18572-114">Identificador MobieApp.</span><span class="sxs-lookup"><span data-stu-id="18572-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="18572-115">displayName</span><span class="sxs-lookup"><span data-stu-id="18572-115">displayName</span></span>|<span data-ttu-id="18572-116">String</span><span class="sxs-lookup"><span data-stu-id="18572-116">String</span></span>|<span data-ttu-id="18572-117">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="18572-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="18572-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="18572-118">mobileAppIntent</span></span>|[<span data-ttu-id="18572-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="18572-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="18572-120">Tentativa de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="18572-120">Mobile App Intent.</span></span> <span data-ttu-id="18572-121">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="18572-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="18572-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="18572-122">displayVersion</span></span>|<span data-ttu-id="18572-123">String</span><span class="sxs-lookup"><span data-stu-id="18572-123">String</span></span>|<span data-ttu-id="18572-124">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="18572-124">Human readable version of the application</span></span>|
|<span data-ttu-id="18572-125">installState</span><span class="sxs-lookup"><span data-stu-id="18572-125">installState</span></span>|[<span data-ttu-id="18572-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="18572-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="18572-127">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18572-127">The install state of the app.</span></span> <span data-ttu-id="18572-128">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="18572-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="18572-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="18572-129">supportedDeviceTypes</span></span>|<span data-ttu-id="18572-130">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="18572-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="18572-131">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="18572-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18572-132">Relações</span><span class="sxs-lookup"><span data-stu-id="18572-132">Relationships</span></span>
<span data-ttu-id="18572-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18572-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18572-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18572-134">JSON Representation</span></span>
<span data-ttu-id="18572-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18572-135">Here is a JSON representation of the resource.</span></span>
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






