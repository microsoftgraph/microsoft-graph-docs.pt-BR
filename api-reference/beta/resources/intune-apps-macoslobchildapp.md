---
title: tipo de recurso de macOSLobChildApp
description: Contém propriedades o MacOS LOB App em um pacote de pacote
author: tfitzmac
ms.openlocfilehash: e62305ea856d42847b49be306d20bde737152163
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27309867"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="18ff8-103">tipo de recurso de macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="18ff8-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="18ff8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="18ff8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="18ff8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="18ff8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="18ff8-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="18ff8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18ff8-107">Contém propriedades o MacOS LOB App em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="18ff8-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="18ff8-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18ff8-108">Properties</span></span>
|<span data-ttu-id="18ff8-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18ff8-109">Property</span></span>|<span data-ttu-id="18ff8-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="18ff8-110">Type</span></span>|<span data-ttu-id="18ff8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="18ff8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18ff8-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="18ff8-112">bundleId</span></span>|<span data-ttu-id="18ff8-113">String</span><span class="sxs-lookup"><span data-stu-id="18ff8-113">String</span></span>|<span data-ttu-id="18ff8-114">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="18ff8-114">The Identity Name.</span></span>|
|<span data-ttu-id="18ff8-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="18ff8-115">buildNumber</span></span>|<span data-ttu-id="18ff8-116">String</span><span class="sxs-lookup"><span data-stu-id="18ff8-116">String</span></span>|<span data-ttu-id="18ff8-117">O número de compilação da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="18ff8-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="18ff8-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="18ff8-118">versionNumber</span></span>|<span data-ttu-id="18ff8-119">String</span><span class="sxs-lookup"><span data-stu-id="18ff8-119">String</span></span>|<span data-ttu-id="18ff8-120">O número de versão da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="18ff8-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18ff8-121">Relações</span><span class="sxs-lookup"><span data-stu-id="18ff8-121">Relationships</span></span>
<span data-ttu-id="18ff8-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="18ff8-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="18ff8-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18ff8-123">JSON Representation</span></span>
<span data-ttu-id="18ff8-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18ff8-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





