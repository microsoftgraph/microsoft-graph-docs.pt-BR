---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cd612a5593ef151d4f324f3058c793ce7cd29bf0
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949630"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="52743-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="52743-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="52743-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52743-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52743-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52743-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52743-106">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="52743-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="52743-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52743-107">Properties</span></span>
|<span data-ttu-id="52743-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52743-108">Property</span></span>|<span data-ttu-id="52743-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="52743-109">Type</span></span>|<span data-ttu-id="52743-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52743-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52743-111">productCode</span><span class="sxs-lookup"><span data-stu-id="52743-111">productCode</span></span>|<span data-ttu-id="52743-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52743-112">String</span></span>|<span data-ttu-id="52743-113">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="52743-113">The MSI product code.</span></span>|
|<span data-ttu-id="52743-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="52743-114">productVersion</span></span>|<span data-ttu-id="52743-115">String</span><span class="sxs-lookup"><span data-stu-id="52743-115">String</span></span>|<span data-ttu-id="52743-116">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="52743-116">The MSI product version.</span></span>|
|<span data-ttu-id="52743-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="52743-117">upgradeCode</span></span>|<span data-ttu-id="52743-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52743-118">String</span></span>|<span data-ttu-id="52743-119">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="52743-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="52743-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="52743-120">requiresReboot</span></span>|<span data-ttu-id="52743-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="52743-121">Boolean</span></span>|<span data-ttu-id="52743-122">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="52743-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="52743-123">PackageType</span><span class="sxs-lookup"><span data-stu-id="52743-123">packageType</span></span>|[<span data-ttu-id="52743-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="52743-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="52743-125">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="52743-125">The MSI package type.</span></span> <span data-ttu-id="52743-126">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="52743-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="52743-127">productName</span><span class="sxs-lookup"><span data-stu-id="52743-127">productName</span></span>|<span data-ttu-id="52743-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52743-128">String</span></span>|<span data-ttu-id="52743-129">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="52743-129">The MSI product name.</span></span>|
|<span data-ttu-id="52743-130">publicador</span><span class="sxs-lookup"><span data-stu-id="52743-130">publisher</span></span>|<span data-ttu-id="52743-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52743-131">String</span></span>|<span data-ttu-id="52743-132">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="52743-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52743-133">Relações</span><span class="sxs-lookup"><span data-stu-id="52743-133">Relationships</span></span>
<span data-ttu-id="52743-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52743-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52743-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52743-135">JSON Representation</span></span>
<span data-ttu-id="52743-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52743-136">Here is a JSON representation of the resource.</span></span>
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




