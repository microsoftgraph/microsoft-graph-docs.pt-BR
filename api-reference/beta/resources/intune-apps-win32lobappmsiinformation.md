---
title: tipo de recurso de win32LobAppMsiInformation
description: Contém propriedades de app MSI para um aplicativo Win32.
author: tfitzmac
ms.openlocfilehash: 1753df68ab1f4b0e1649c16a4a7fa0ad49941bf9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326135"
---
# <a name="win32lobappmsiinformation-resource-type"></a><span data-ttu-id="9972e-103">tipo de recurso de win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="9972e-103">win32LobAppMsiInformation resource type</span></span>

> <span data-ttu-id="9972e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="9972e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9972e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9972e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9972e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9972e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9972e-107">Contém propriedades de app MSI para um aplicativo Win32.</span><span class="sxs-lookup"><span data-stu-id="9972e-107">Contains MSI app properties for a Win32 App.</span></span>
## <a name="properties"></a><span data-ttu-id="9972e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9972e-108">Properties</span></span>
|<span data-ttu-id="9972e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9972e-109">Property</span></span>|<span data-ttu-id="9972e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9972e-110">Type</span></span>|<span data-ttu-id="9972e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9972e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9972e-112">productCode</span><span class="sxs-lookup"><span data-stu-id="9972e-112">productCode</span></span>|<span data-ttu-id="9972e-113">String</span><span class="sxs-lookup"><span data-stu-id="9972e-113">String</span></span>|<span data-ttu-id="9972e-114">O código do produto MSI.</span><span class="sxs-lookup"><span data-stu-id="9972e-114">The MSI product code.</span></span>|
|<span data-ttu-id="9972e-115">productVersion</span><span class="sxs-lookup"><span data-stu-id="9972e-115">productVersion</span></span>|<span data-ttu-id="9972e-116">String</span><span class="sxs-lookup"><span data-stu-id="9972e-116">String</span></span>|<span data-ttu-id="9972e-117">A versão MSI do produto.</span><span class="sxs-lookup"><span data-stu-id="9972e-117">The MSI product version.</span></span>|
|<span data-ttu-id="9972e-118">upgradeCode</span><span class="sxs-lookup"><span data-stu-id="9972e-118">upgradeCode</span></span>|<span data-ttu-id="9972e-119">String</span><span class="sxs-lookup"><span data-stu-id="9972e-119">String</span></span>|<span data-ttu-id="9972e-120">O código de atualização de MSI.</span><span class="sxs-lookup"><span data-stu-id="9972e-120">The MSI upgrade code.</span></span>|
|<span data-ttu-id="9972e-121">requiresReboot</span><span class="sxs-lookup"><span data-stu-id="9972e-121">requiresReboot</span></span>|<span data-ttu-id="9972e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="9972e-122">Boolean</span></span>|<span data-ttu-id="9972e-123">Se o aplicativo MSI requer a máquina reinicie para concluir a instalação.</span><span class="sxs-lookup"><span data-stu-id="9972e-123">Whether the MSI app requires the machine to reboot to complete installation.</span></span>|
|<span data-ttu-id="9972e-124">tipo de pacote</span><span class="sxs-lookup"><span data-stu-id="9972e-124">packageType</span></span>|[<span data-ttu-id="9972e-125">win32LobAppMsiPackageType</span><span class="sxs-lookup"><span data-stu-id="9972e-125">win32LobAppMsiPackageType</span></span>](../resources/intune-apps-win32lobappmsipackagetype.md)|<span data-ttu-id="9972e-126">O tipo de pacote MSI.</span><span class="sxs-lookup"><span data-stu-id="9972e-126">The MSI package type.</span></span> <span data-ttu-id="9972e-127">Os valores possíveis são: `perMachine`, `perUser`, `dualPurpose`.</span><span class="sxs-lookup"><span data-stu-id="9972e-127">Possible values are: `perMachine`, `perUser`, `dualPurpose`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9972e-128">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9972e-128">Relationships</span></span>
<span data-ttu-id="9972e-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9972e-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9972e-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9972e-130">JSON Representation</span></span>
<span data-ttu-id="9972e-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9972e-131">Here is a JSON representation of the resource.</span></span>
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





