---
title: tipo de recurso mobileAppIntentAndStateDetail
description: Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 62071f73a670d3281dade4e555203abe9ed21e3e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48730287"
---
# <a name="mobileappintentandstatedetail-resource-type"></a><span data-ttu-id="b0bcf-103">tipo de recurso mobileAppIntentAndStateDetail</span><span class="sxs-lookup"><span data-stu-id="b0bcf-103">mobileAppIntentAndStateDetail resource type</span></span>

<span data-ttu-id="b0bcf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0bcf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0bcf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0bcf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0bcf-107">Tentativa de aplicativo móvel e estado de instalação para um determinado dispositivo.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-107">Mobile App Intent and Install State for a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b0bcf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b0bcf-108">Properties</span></span>
|<span data-ttu-id="b0bcf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b0bcf-109">Property</span></span>|<span data-ttu-id="b0bcf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b0bcf-110">Type</span></span>|<span data-ttu-id="b0bcf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b0bcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0bcf-112">ApplicationId</span><span class="sxs-lookup"><span data-stu-id="b0bcf-112">applicationId</span></span>|<span data-ttu-id="b0bcf-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b0bcf-113">String</span></span>|<span data-ttu-id="b0bcf-114">Identificador MobieApp.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-114">MobieApp identifier.</span></span>|
|<span data-ttu-id="b0bcf-115">displayName</span><span class="sxs-lookup"><span data-stu-id="b0bcf-115">displayName</span></span>|<span data-ttu-id="b0bcf-116">String</span><span class="sxs-lookup"><span data-stu-id="b0bcf-116">String</span></span>|<span data-ttu-id="b0bcf-117">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-117">The admin provided or imported title of the app.</span></span>|
|<span data-ttu-id="b0bcf-118">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="b0bcf-118">mobileAppIntent</span></span>|[<span data-ttu-id="b0bcf-119">mobileAppIntent</span><span class="sxs-lookup"><span data-stu-id="b0bcf-119">mobileAppIntent</span></span>](../resources/intune-troubleshooting-mobileappintent.md)|<span data-ttu-id="b0bcf-120">Tentativa de aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-120">Mobile App Intent.</span></span> <span data-ttu-id="b0bcf-121">Os valores possíveis são: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-121">Possible values are: `available`, `notAvailable`, `requiredInstall`, `requiredUninstall`, `requiredAndAvailableInstall`, `availableInstallWithoutEnrollment`, `exclude`.</span></span>|
|<span data-ttu-id="b0bcf-122">displayVersion</span><span class="sxs-lookup"><span data-stu-id="b0bcf-122">displayVersion</span></span>|<span data-ttu-id="b0bcf-123">String</span><span class="sxs-lookup"><span data-stu-id="b0bcf-123">String</span></span>|<span data-ttu-id="b0bcf-124">Versão de leitura humana do aplicativo</span><span class="sxs-lookup"><span data-stu-id="b0bcf-124">Human readable version of the application</span></span>|
|<span data-ttu-id="b0bcf-125">installState</span><span class="sxs-lookup"><span data-stu-id="b0bcf-125">installState</span></span>|[<span data-ttu-id="b0bcf-126">resultantAppState</span><span class="sxs-lookup"><span data-stu-id="b0bcf-126">resultantAppState</span></span>](../resources/intune-shared-resultantappstate.md)|<span data-ttu-id="b0bcf-127">O estado de instalação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-127">The install state of the app.</span></span> <span data-ttu-id="b0bcf-128">Os valores possíveis são: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-128">Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.</span></span>|
|<span data-ttu-id="b0bcf-129">supportedDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="b0bcf-129">supportedDeviceTypes</span></span>|<span data-ttu-id="b0bcf-130">coleção [mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md)</span><span class="sxs-lookup"><span data-stu-id="b0bcf-130">[mobileAppSupportedDeviceType](../resources/intune-troubleshooting-mobileappsupporteddevicetype.md) collection</span></span>|<span data-ttu-id="b0bcf-131">As plataformas com suporte para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-131">The supported platforms for the app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0bcf-132">Relações</span><span class="sxs-lookup"><span data-stu-id="b0bcf-132">Relationships</span></span>
<span data-ttu-id="b0bcf-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b0bcf-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0bcf-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b0bcf-134">JSON Representation</span></span>
<span data-ttu-id="b0bcf-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b0bcf-135">Here is a JSON representation of the resource.</span></span>
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





