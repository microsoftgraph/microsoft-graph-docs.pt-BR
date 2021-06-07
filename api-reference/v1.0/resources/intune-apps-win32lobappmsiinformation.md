---
title: Tipo de recurso win32LobAppMsiInformation
description: Contém propriedades de aplicativo MSI para um aplicativo Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f9c610711f58a9d1929d0e708e127e2b337396f8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752193"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="ff9f1-103">Tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="ff9f1-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="ff9f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff9f1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff9f1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff9f1-106">Contém propriedades de aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-106">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="ff9f1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff9f1-107">Properties</span></span>
|<span data-ttu-id="ff9f1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff9f1-108">Property</span></span>|<span data-ttu-id="ff9f1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff9f1-109">Type</span></span>|<span data-ttu-id="ff9f1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff9f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff9f1-111">productCode</span><span class="sxs-lookup"><span data-stu-id="ff9f1-111">productCode</span></span>|<span data-ttu-id="ff9f1-112">String</span><span class="sxs-lookup"><span data-stu-id="ff9f1-112">String</span></span>|<span data-ttu-id="ff9f1-113">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-113">The MSI product code.</span></span>|
|<span data-ttu-id="ff9f1-114">productVersion</span><span class="sxs-lookup"><span data-stu-id="ff9f1-114">productVersion</span></span>|<span data-ttu-id="ff9f1-115">String</span><span class="sxs-lookup"><span data-stu-id="ff9f1-115">String</span></span>|<span data-ttu-id="ff9f1-116">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-116">The MSI product version.</span></span>|
|<span data-ttu-id="ff9f1-117">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="ff9f1-117">upgradeCode</span></span>|<span data-ttu-id="ff9f1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff9f1-118">String</span></span>|<span data-ttu-id="ff9f1-119">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-119">The MSI upgrade code.</span></span>|
|<span data-ttu-id="ff9f1-120">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="ff9f1-120">requiresReboot</span></span>|<span data-ttu-id="ff9f1-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="ff9f1-121">Boolean</span></span>|<span data-ttu-id="ff9f1-122">Se o aplicativo MSI exige que o computador seja reiniciado para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-122">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="ff9f1-123">packageType</span><span class="sxs-lookup"><span data-stu-id="ff9f1-123">packageType</span></span>|[<span data-ttu-id="ff9f1-124">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="ff9f1-124">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="ff9f1-125">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-125">The MSI package type.</span></span> <span data-ttu-id="ff9f1-126">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-126">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="ff9f1-127">productName</span><span class="sxs-lookup"><span data-stu-id="ff9f1-127">productName</span></span>|<span data-ttu-id="ff9f1-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff9f1-128">String</span></span>|<span data-ttu-id="ff9f1-129">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-129">The MSI product name.</span></span>|
|<span data-ttu-id="ff9f1-130">publicador</span><span class="sxs-lookup"><span data-stu-id="ff9f1-130">publisher</span></span>|<span data-ttu-id="ff9f1-131">String</span><span class="sxs-lookup"><span data-stu-id="ff9f1-131">String</span></span>|<span data-ttu-id="ff9f1-132">O editor MSI.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-132">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff9f1-133">Relações</span><span class="sxs-lookup"><span data-stu-id="ff9f1-133">Relationships</span></span>
<span data-ttu-id="ff9f1-134">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ff9f1-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff9f1-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff9f1-135">JSON Representation</span></span>
<span data-ttu-id="ff9f1-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff9f1-136">Here is a JSON representation of the resource.</span></span>
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




