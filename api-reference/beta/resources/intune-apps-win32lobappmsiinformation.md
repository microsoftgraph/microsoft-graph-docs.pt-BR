---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3ddb69d3f01c816c592617cb75ed6f9b9877f856
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534483"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="d924b-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="d924b-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="d924b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d924b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d924b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d924b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d924b-106">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="d924b-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="d924b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d924b-107">Properties</span></span>
|<span data-ttu-id="d924b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d924b-108">Property</span></span>|<span data-ttu-id="d924b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d924b-109">Type</span></span>|<span data-ttu-id="d924b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d924b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d924b-111">productCode</span><span class="sxs-lookup"><span data-stu-id="d924b-111">productCode</span></span>|<span data-ttu-id="d924b-112">String</span><span class="sxs-lookup"><span data-stu-id="d924b-112">String</span></span>|<span data-ttu-id="d924b-113">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="d924b-113">The MSI product code.</span></span>|
|<span data-ttu-id="d924b-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="d924b-114">productVersion</span></span>|<span data-ttu-id="d924b-115">String</span><span class="sxs-lookup"><span data-stu-id="d924b-115">String</span></span>|<span data-ttu-id="d924b-116">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="d924b-116">The MSI product version.</span></span>|
|<span data-ttu-id="d924b-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="d924b-117">upgradeCode</span></span>|<span data-ttu-id="d924b-118">String</span><span class="sxs-lookup"><span data-stu-id="d924b-118">String</span></span>|<span data-ttu-id="d924b-119">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="d924b-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="d924b-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="d924b-120">requiresReboot</span></span>|<span data-ttu-id="d924b-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="d924b-121">Boolean</span></span>|<span data-ttu-id="d924b-122">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="d924b-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="d924b-123">PackageType</span><span class="sxs-lookup"><span data-stu-id="d924b-123">packageType</span></span>|[<span data-ttu-id="d924b-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="d924b-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="d924b-125">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="d924b-125">The MSI package type.</span></span> <span data-ttu-id="d924b-126">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="d924b-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="d924b-127">productName</span><span class="sxs-lookup"><span data-stu-id="d924b-127">productName</span></span>|<span data-ttu-id="d924b-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d924b-128">String</span></span>|<span data-ttu-id="d924b-129">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="d924b-129">The MSI product name.</span></span>|
|<span data-ttu-id="d924b-130">publicador</span><span class="sxs-lookup"><span data-stu-id="d924b-130">publisher</span></span>|<span data-ttu-id="d924b-131">String</span><span class="sxs-lookup"><span data-stu-id="d924b-131">String</span></span>|<span data-ttu-id="d924b-132">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="d924b-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d924b-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d924b-133">Relationships</span></span>
<span data-ttu-id="d924b-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d924b-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d924b-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d924b-135">JSON Representation</span></span>
<span data-ttu-id="d924b-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d924b-136">Here is a JSON representation of the resource.</span></span>
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





