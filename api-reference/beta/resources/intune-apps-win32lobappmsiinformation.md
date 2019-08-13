---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 958cc834a2044e623a8fa1cf7ed37bed1ec7b1f9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36335645"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="11deb-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="11deb-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="11deb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="11deb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11deb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="11deb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11deb-106">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="11deb-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="11deb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11deb-107">Properties</span></span>
|<span data-ttu-id="11deb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11deb-108">Property</span></span>|<span data-ttu-id="11deb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="11deb-109">Type</span></span>|<span data-ttu-id="11deb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="11deb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11deb-111">productCode</span><span class="sxs-lookup"><span data-stu-id="11deb-111">productCode</span></span>|<span data-ttu-id="11deb-112">String</span><span class="sxs-lookup"><span data-stu-id="11deb-112">String</span></span>|<span data-ttu-id="11deb-113">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="11deb-113">The MSI product code.</span></span>|
|<span data-ttu-id="11deb-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="11deb-114">productVersion</span></span>|<span data-ttu-id="11deb-115">String</span><span class="sxs-lookup"><span data-stu-id="11deb-115">String</span></span>|<span data-ttu-id="11deb-116">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="11deb-116">The MSI product version.</span></span>|
|<span data-ttu-id="11deb-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="11deb-117">upgradeCode</span></span>|<span data-ttu-id="11deb-118">String</span><span class="sxs-lookup"><span data-stu-id="11deb-118">String</span></span>|<span data-ttu-id="11deb-119">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="11deb-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="11deb-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="11deb-120">requiresReboot</span></span>|<span data-ttu-id="11deb-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="11deb-121">Boolean</span></span>|<span data-ttu-id="11deb-122">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="11deb-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="11deb-123">PackageType</span><span class="sxs-lookup"><span data-stu-id="11deb-123">packageType</span></span>|[<span data-ttu-id="11deb-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="11deb-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="11deb-125">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="11deb-125">The MSI package type.</span></span> <span data-ttu-id="11deb-126">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="11deb-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="11deb-127">productName</span><span class="sxs-lookup"><span data-stu-id="11deb-127">productName</span></span>|<span data-ttu-id="11deb-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="11deb-128">String</span></span>|<span data-ttu-id="11deb-129">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="11deb-129">The MSI product name.</span></span>|
|<span data-ttu-id="11deb-130">publicador</span><span class="sxs-lookup"><span data-stu-id="11deb-130">publisher</span></span>|<span data-ttu-id="11deb-131">String</span><span class="sxs-lookup"><span data-stu-id="11deb-131">String</span></span>|<span data-ttu-id="11deb-132">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="11deb-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="11deb-133">Relações</span><span class="sxs-lookup"><span data-stu-id="11deb-133">Relationships</span></span>
<span data-ttu-id="11deb-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="11deb-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11deb-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11deb-135">JSON Representation</span></span>
<span data-ttu-id="11deb-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11deb-136">Here is a JSON representation of the resource.</span></span>
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



