---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fd710b166bd1171ed17a2deef7648e580d578301
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797637"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="94d98-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="94d98-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="94d98-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94d98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94d98-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94d98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94d98-106">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="94d98-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="94d98-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94d98-107">Properties</span></span>
|<span data-ttu-id="94d98-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94d98-108">Property</span></span>|<span data-ttu-id="94d98-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="94d98-109">Type</span></span>|<span data-ttu-id="94d98-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94d98-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94d98-111">productCode</span><span class="sxs-lookup"><span data-stu-id="94d98-111">productCode</span></span>|<span data-ttu-id="94d98-112">String</span><span class="sxs-lookup"><span data-stu-id="94d98-112">String</span></span>|<span data-ttu-id="94d98-113">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="94d98-113">The MSI product code.</span></span>|
|<span data-ttu-id="94d98-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="94d98-114">productVersion</span></span>|<span data-ttu-id="94d98-115">String</span><span class="sxs-lookup"><span data-stu-id="94d98-115">String</span></span>|<span data-ttu-id="94d98-116">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="94d98-116">The MSI product version.</span></span>|
|<span data-ttu-id="94d98-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="94d98-117">upgradeCode</span></span>|<span data-ttu-id="94d98-118">String</span><span class="sxs-lookup"><span data-stu-id="94d98-118">String</span></span>|<span data-ttu-id="94d98-119">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="94d98-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="94d98-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="94d98-120">requiresReboot</span></span>|<span data-ttu-id="94d98-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="94d98-121">Boolean</span></span>|<span data-ttu-id="94d98-122">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="94d98-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="94d98-123">PackageType</span><span class="sxs-lookup"><span data-stu-id="94d98-123">packageType</span></span>|[<span data-ttu-id="94d98-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="94d98-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="94d98-125">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="94d98-125">The MSI package type.</span></span> <span data-ttu-id="94d98-126">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="94d98-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="94d98-127">productName</span><span class="sxs-lookup"><span data-stu-id="94d98-127">productName</span></span>|<span data-ttu-id="94d98-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94d98-128">String</span></span>|<span data-ttu-id="94d98-129">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="94d98-129">The MSI product name.</span></span>|
|<span data-ttu-id="94d98-130">publicador</span><span class="sxs-lookup"><span data-stu-id="94d98-130">publisher</span></span>|<span data-ttu-id="94d98-131">String</span><span class="sxs-lookup"><span data-stu-id="94d98-131">String</span></span>|<span data-ttu-id="94d98-132">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="94d98-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94d98-133">Relações</span><span class="sxs-lookup"><span data-stu-id="94d98-133">Relationships</span></span>
<span data-ttu-id="94d98-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94d98-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94d98-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94d98-135">JSON Representation</span></span>
<span data-ttu-id="94d98-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94d98-136">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppMsiInformation",
  "productCode": "String",
  "productVersion": "String",
  "upgradeCode": "String",
  "requiresReboot": true,
  "packageType": "String",
  "productName": "String",
  "publisher": "String"
}
```



