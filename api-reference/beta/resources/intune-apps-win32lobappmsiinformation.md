---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f330111a3e924e54cf23c30cd98d20e85cb38022
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158643"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="45d09-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="45d09-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="45d09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45d09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45d09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45d09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45d09-106">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="45d09-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="45d09-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45d09-107">Properties</span></span>
|<span data-ttu-id="45d09-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45d09-108">Property</span></span>|<span data-ttu-id="45d09-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="45d09-109">Type</span></span>|<span data-ttu-id="45d09-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="45d09-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45d09-111">productCode</span><span class="sxs-lookup"><span data-stu-id="45d09-111">productCode</span></span>|<span data-ttu-id="45d09-112">String</span><span class="sxs-lookup"><span data-stu-id="45d09-112">String</span></span>|<span data-ttu-id="45d09-113">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="45d09-113">The MSI product code.</span></span>|
|<span data-ttu-id="45d09-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="45d09-114">productVersion</span></span>|<span data-ttu-id="45d09-115">String</span><span class="sxs-lookup"><span data-stu-id="45d09-115">String</span></span>|<span data-ttu-id="45d09-116">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="45d09-116">The MSI product version.</span></span>|
|<span data-ttu-id="45d09-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="45d09-117">upgradeCode</span></span>|<span data-ttu-id="45d09-118">String</span><span class="sxs-lookup"><span data-stu-id="45d09-118">String</span></span>|<span data-ttu-id="45d09-119">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="45d09-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="45d09-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="45d09-120">requiresReboot</span></span>|<span data-ttu-id="45d09-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="45d09-121">Boolean</span></span>|<span data-ttu-id="45d09-122">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="45d09-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="45d09-123">PackageType</span><span class="sxs-lookup"><span data-stu-id="45d09-123">packageType</span></span>|[<span data-ttu-id="45d09-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="45d09-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="45d09-125">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="45d09-125">The MSI package type.</span></span> <span data-ttu-id="45d09-126">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="45d09-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="45d09-127">productName</span><span class="sxs-lookup"><span data-stu-id="45d09-127">productName</span></span>|<span data-ttu-id="45d09-128">String</span><span class="sxs-lookup"><span data-stu-id="45d09-128">String</span></span>|<span data-ttu-id="45d09-129">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="45d09-129">The MSI product name.</span></span>|
|<span data-ttu-id="45d09-130">publisher</span><span class="sxs-lookup"><span data-stu-id="45d09-130">publisher</span></span>|<span data-ttu-id="45d09-131">String</span><span class="sxs-lookup"><span data-stu-id="45d09-131">String</span></span>|<span data-ttu-id="45d09-132">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="45d09-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45d09-133">Relações</span><span class="sxs-lookup"><span data-stu-id="45d09-133">Relationships</span></span>
<span data-ttu-id="45d09-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45d09-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45d09-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45d09-135">JSON Representation</span></span>
<span data-ttu-id="45d09-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45d09-136">Here is a JSON representation of the resource.</span></span>
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




