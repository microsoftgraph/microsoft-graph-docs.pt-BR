---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 151b0d756258b3c1b5911ab8719c3f72a6e7b263
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422963"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="98e94-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="98e94-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="98e94-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98e94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="98e94-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="98e94-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="98e94-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="98e94-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="98e94-107">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="98e94-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="98e94-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="98e94-108">Properties</span></span>
|<span data-ttu-id="98e94-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="98e94-109">Property</span></span>|<span data-ttu-id="98e94-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="98e94-110">Type</span></span>|<span data-ttu-id="98e94-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="98e94-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="98e94-112">productCode</span><span class="sxs-lookup"><span data-stu-id="98e94-112">productCode</span></span>|<span data-ttu-id="98e94-113">String</span><span class="sxs-lookup"><span data-stu-id="98e94-113">String</span></span>|<span data-ttu-id="98e94-114">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="98e94-114">The MSI product code.</span></span>|
|<span data-ttu-id="98e94-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="98e94-115">productVersion</span></span>|<span data-ttu-id="98e94-116">String</span><span class="sxs-lookup"><span data-stu-id="98e94-116">String</span></span>|<span data-ttu-id="98e94-117">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="98e94-117">The MSI product version.</span></span>|
|<span data-ttu-id="98e94-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="98e94-118">upgradeCode</span></span>|<span data-ttu-id="98e94-119">String</span><span class="sxs-lookup"><span data-stu-id="98e94-119">String</span></span>|<span data-ttu-id="98e94-120">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="98e94-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="98e94-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="98e94-121">requiresReboot</span></span>|<span data-ttu-id="98e94-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="98e94-122">Boolean</span></span>|<span data-ttu-id="98e94-123">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="98e94-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="98e94-124">PackageType</span><span class="sxs-lookup"><span data-stu-id="98e94-124">packageType</span></span>|[<span data-ttu-id="98e94-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="98e94-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="98e94-126">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="98e94-126">The MSI package type.</span></span> <span data-ttu-id="98e94-127">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="98e94-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="98e94-128">productName</span><span class="sxs-lookup"><span data-stu-id="98e94-128">productName</span></span>|<span data-ttu-id="98e94-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="98e94-129">String</span></span>|<span data-ttu-id="98e94-130">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="98e94-130">The MSI product name.</span></span>|
|<span data-ttu-id="98e94-131">publicador</span><span class="sxs-lookup"><span data-stu-id="98e94-131">publisher</span></span>|<span data-ttu-id="98e94-132">String</span><span class="sxs-lookup"><span data-stu-id="98e94-132">String</span></span>|<span data-ttu-id="98e94-133">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="98e94-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98e94-134">Relações</span><span class="sxs-lookup"><span data-stu-id="98e94-134">Relationships</span></span>
<span data-ttu-id="98e94-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="98e94-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="98e94-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="98e94-136">JSON Representation</span></span>
<span data-ttu-id="98e94-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="98e94-137">Here is a JSON representation of the resource.</span></span>
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



