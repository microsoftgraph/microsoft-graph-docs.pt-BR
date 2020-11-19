---
title: tipo de recurso win32LobAppMsiInformation
description: Contém as propriedades do aplicativo MSI para um aplicativo Win32.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fb872d970256a795c51570d68b3279fce43506f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274002"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="f7f7e-103">tipo de recurso win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="f7f7e-103">win32LobAppMsiInformation resource type</span></span>

<span data-ttu-id="f7f7e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7f7e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7f7e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7f7e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7f7e-107">Contém as propriedades do aplicativo MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="f7f7e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7f7e-108">Properties</span></span>
|<span data-ttu-id="f7f7e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7f7e-109">Property</span></span>|<span data-ttu-id="f7f7e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7f7e-110">Type</span></span>|<span data-ttu-id="f7f7e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7f7e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7f7e-112">productCode</span><span class="sxs-lookup"><span data-stu-id="f7f7e-112">productCode</span></span>|<span data-ttu-id="f7f7e-113">String</span><span class="sxs-lookup"><span data-stu-id="f7f7e-113">String</span></span>|<span data-ttu-id="f7f7e-114">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-114">The MSI product code.</span></span>|
|<span data-ttu-id="f7f7e-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="f7f7e-115">productVersion</span></span>|<span data-ttu-id="f7f7e-116">String</span><span class="sxs-lookup"><span data-stu-id="f7f7e-116">String</span></span>|<span data-ttu-id="f7f7e-117">A versão do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-117">The MSI product version.</span></span>|
|<span data-ttu-id="f7f7e-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="f7f7e-118">upgradeCode</span></span>|<span data-ttu-id="f7f7e-119">String</span><span class="sxs-lookup"><span data-stu-id="f7f7e-119">String</span></span>|<span data-ttu-id="f7f7e-120">O código de atualização MSI.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="f7f7e-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="f7f7e-121">requiresReboot</span></span>|<span data-ttu-id="f7f7e-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7f7e-122">Boolean</span></span>|<span data-ttu-id="f7f7e-123">Se o aplicativo MSI exige a reinicialização do computador para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="f7f7e-124">PackageType</span><span class="sxs-lookup"><span data-stu-id="f7f7e-124">packageType</span></span>|[<span data-ttu-id="f7f7e-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="f7f7e-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="f7f7e-126">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-126">The MSI package type.</span></span> <span data-ttu-id="f7f7e-127">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|
|<span data-ttu-id="f7f7e-128">productName</span><span class="sxs-lookup"><span data-stu-id="f7f7e-128">productName</span></span>|<span data-ttu-id="f7f7e-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f7f7e-129">String</span></span>|<span data-ttu-id="f7f7e-130">O nome do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-130">The MSI product name.</span></span>|
|<span data-ttu-id="f7f7e-131">publicador</span><span class="sxs-lookup"><span data-stu-id="f7f7e-131">publisher</span></span>|<span data-ttu-id="f7f7e-132">String</span><span class="sxs-lookup"><span data-stu-id="f7f7e-132">String</span></span>|<span data-ttu-id="f7f7e-133">O Publicador MSI.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-133">The MSI publisher.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7f7e-134">Relações</span><span class="sxs-lookup"><span data-stu-id="f7f7e-134">Relationships</span></span>
<span data-ttu-id="f7f7e-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7f7e-135">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7f7e-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7f7e-136">JSON Representation</span></span>
<span data-ttu-id="f7f7e-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7f7e-137">Here is a JSON representation of the resource.</span></span>
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




