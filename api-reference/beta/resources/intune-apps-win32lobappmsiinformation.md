---
title: tipo de recurso de win32LobAppMsiInformation
description: Contém propriedades de app MSI para um aplicativo Win32.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04972e9e7fa909c220fe55ca6337be3ac44138ad
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967872"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="7495d-103">tipo de recurso de win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="7495d-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="7495d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="7495d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7495d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7495d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7495d-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="7495d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7495d-107">Contém propriedades de app MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="7495d-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="7495d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7495d-108">Properties</span></span>
|<span data-ttu-id="7495d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7495d-109">Property</span></span>|<span data-ttu-id="7495d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7495d-110">Type</span></span>|<span data-ttu-id="7495d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7495d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7495d-112">productCode</span><span class="sxs-lookup"><span data-stu-id="7495d-112">productCode</span></span>|<span data-ttu-id="7495d-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7495d-113">String</span></span>|<span data-ttu-id="7495d-114">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="7495d-114">The MSI product code.</span></span>|
|<span data-ttu-id="7495d-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="7495d-115">productVersion</span></span>|<span data-ttu-id="7495d-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7495d-116">String</span></span>|<span data-ttu-id="7495d-117">A versão MSI do produto.</span><span class="sxs-lookup"><span data-stu-id="7495d-117">The MSI product version.</span></span>|
|<span data-ttu-id="7495d-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="7495d-118">upgradeCode</span></span>|<span data-ttu-id="7495d-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7495d-119">String</span></span>|<span data-ttu-id="7495d-120">O código de atualização de MSI.</span><span class="sxs-lookup"><span data-stu-id="7495d-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="7495d-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="7495d-121">requiresReboot</span></span>|<span data-ttu-id="7495d-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="7495d-122">Boolean</span></span>|<span data-ttu-id="7495d-123">Se o aplicativo MSI requer a máquina reinicie para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="7495d-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="7495d-124">tipo de pacote</span><span class="sxs-lookup"><span data-stu-id="7495d-124">packageType</span></span>|[<span data-ttu-id="7495d-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="7495d-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="7495d-126">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="7495d-126">The MSI package type.</span></span> <span data-ttu-id="7495d-127">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="7495d-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7495d-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="7495d-128">Relationships</span></span>
<span data-ttu-id="7495d-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7495d-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7495d-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7495d-130">JSON Representation</span></span>
<span data-ttu-id="7495d-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7495d-131">Here is a JSON representation of the resource.</span></span>
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





