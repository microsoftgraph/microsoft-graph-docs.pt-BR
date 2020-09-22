---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8553fb6b2efafd7ede072456ef99271e3df0ea09
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033703"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="3b800-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="3b800-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="3b800-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b800-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b800-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b800-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b800-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b800-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b800-107">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="3b800-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="3b800-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b800-108">Properties</span></span>
|<span data-ttu-id="3b800-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b800-109">Property</span></span>|<span data-ttu-id="3b800-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b800-110">Type</span></span>|<span data-ttu-id="3b800-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b800-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b800-112">productCode</span><span class="sxs-lookup"><span data-stu-id="3b800-112">productCode</span></span>|<span data-ttu-id="3b800-113">String</span><span class="sxs-lookup"><span data-stu-id="3b800-113">String</span></span>|<span data-ttu-id="3b800-114">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="3b800-114">The MSI product code.</span></span>|
|<span data-ttu-id="3b800-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="3b800-115">productVersion</span></span>|<span data-ttu-id="3b800-116">String</span><span class="sxs-lookup"><span data-stu-id="3b800-116">String</span></span>|<span data-ttu-id="3b800-117">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="3b800-117">The MSI product version.</span></span>|
|<span data-ttu-id="3b800-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="3b800-118">upgradeCode</span></span>|<span data-ttu-id="3b800-119">String</span><span class="sxs-lookup"><span data-stu-id="3b800-119">String</span></span>|<span data-ttu-id="3b800-120">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="3b800-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="3b800-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="3b800-121">requiresReboot</span></span>|<span data-ttu-id="3b800-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="3b800-122">Boolean</span></span>|<span data-ttu-id="3b800-123">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="3b800-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="3b800-124">PackageType</span><span class="sxs-lookup"><span data-stu-id="3b800-124">packageType</span></span>|[<span data-ttu-id="3b800-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="3b800-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="3b800-126">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="3b800-126">The MSI package type.</span></span> <span data-ttu-id="3b800-127">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="3b800-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="3b800-128">productName</span><span class="sxs-lookup"><span data-stu-id="3b800-128">productName</span></span>|<span data-ttu-id="3b800-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b800-129">String</span></span>|<span data-ttu-id="3b800-130">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="3b800-130">The MSI product name.</span></span>|
|<span data-ttu-id="3b800-131">publicador</span><span class="sxs-lookup"><span data-stu-id="3b800-131">publisher</span></span>|<span data-ttu-id="3b800-132">String</span><span class="sxs-lookup"><span data-stu-id="3b800-132">String</span></span>|<span data-ttu-id="3b800-133">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="3b800-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b800-134">Relações</span><span class="sxs-lookup"><span data-stu-id="3b800-134">Relationships</span></span>
<span data-ttu-id="3b800-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b800-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b800-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b800-136">JSON Representation</span></span>
<span data-ttu-id="3b800-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b800-137">Here is a JSON representation of the resource.</span></span>
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






