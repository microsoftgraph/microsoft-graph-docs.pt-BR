---
title: tipo de recurso de win32LobAppMsiInformation
description: Contém propriedades de app MSI para um aplicativo Win32.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5ba91c572286020a3e349527f325d22bf0be5d67
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399245"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="eaf17-103">tipo de recurso de win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="eaf17-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="eaf17-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="eaf17-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eaf17-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eaf17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eaf17-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="eaf17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eaf17-107">Contém propriedades de app MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="eaf17-107">Contains MSI app properties for a Win32 App.</span></span>

## <a name="properties"></a><span data-ttu-id="eaf17-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eaf17-108">Properties</span></span>
|<span data-ttu-id="eaf17-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eaf17-109">Property</span></span>|<span data-ttu-id="eaf17-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eaf17-110">Type</span></span>|<span data-ttu-id="eaf17-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eaf17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eaf17-112">productCode</span><span class="sxs-lookup"><span data-stu-id="eaf17-112">productCode</span></span>|<span data-ttu-id="eaf17-113">String</span><span class="sxs-lookup"><span data-stu-id="eaf17-113">String</span></span>|<span data-ttu-id="eaf17-114">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="eaf17-114">The MSI product code.</span></span>|
|<span data-ttu-id="eaf17-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="eaf17-115">productVersion</span></span>|<span data-ttu-id="eaf17-116">String</span><span class="sxs-lookup"><span data-stu-id="eaf17-116">String</span></span>|<span data-ttu-id="eaf17-117">A versão MSI do produto.</span><span class="sxs-lookup"><span data-stu-id="eaf17-117">The MSI product version.</span></span>|
|<span data-ttu-id="eaf17-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="eaf17-118">upgradeCode</span></span>|<span data-ttu-id="eaf17-119">String</span><span class="sxs-lookup"><span data-stu-id="eaf17-119">String</span></span>|<span data-ttu-id="eaf17-120">O código de atualização de MSI.</span><span class="sxs-lookup"><span data-stu-id="eaf17-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="eaf17-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="eaf17-121">requiresReboot</span></span>|<span data-ttu-id="eaf17-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="eaf17-122">Boolean</span></span>|<span data-ttu-id="eaf17-123">Se o aplicativo MSI requer a máquina reinicie para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="eaf17-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="eaf17-124">tipo de pacote</span><span class="sxs-lookup"><span data-stu-id="eaf17-124">packageType</span></span>|[<span data-ttu-id="eaf17-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="eaf17-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="eaf17-126">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="eaf17-126">The MSI package type.</span></span> <span data-ttu-id="eaf17-127">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="eaf17-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eaf17-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="eaf17-128">Relationships</span></span>
<span data-ttu-id="eaf17-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eaf17-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eaf17-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eaf17-130">JSON Representation</span></span>
<span data-ttu-id="eaf17-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eaf17-131">Here is a JSON representation of the resource.</span></span>
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
  "packageType": "String"
}
```




