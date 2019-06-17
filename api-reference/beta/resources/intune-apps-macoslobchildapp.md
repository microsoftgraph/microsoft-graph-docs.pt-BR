---
title: tipo de recurso macOSLobChildApp
description: Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 46e84e629f7664f8a5ab33eaa9db6bbc95fd80bc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34957756"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="7479b-103">tipo de recurso macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="7479b-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="7479b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7479b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7479b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7479b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7479b-106">Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="7479b-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="7479b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7479b-107">Properties</span></span>
|<span data-ttu-id="7479b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7479b-108">Property</span></span>|<span data-ttu-id="7479b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7479b-109">Type</span></span>|<span data-ttu-id="7479b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7479b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7479b-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="7479b-111">bundleId</span></span>|<span data-ttu-id="7479b-112">String</span><span class="sxs-lookup"><span data-stu-id="7479b-112">String</span></span>|<span data-ttu-id="7479b-113">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="7479b-113">The Identity Name.</span></span>|
|<span data-ttu-id="7479b-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="7479b-114">buildNumber</span></span>|<span data-ttu-id="7479b-115">String</span><span class="sxs-lookup"><span data-stu-id="7479b-115">String</span></span>|<span data-ttu-id="7479b-116">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="7479b-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="7479b-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="7479b-117">versionNumber</span></span>|<span data-ttu-id="7479b-118">String</span><span class="sxs-lookup"><span data-stu-id="7479b-118">String</span></span>|<span data-ttu-id="7479b-119">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="7479b-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7479b-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7479b-120">Relationships</span></span>
<span data-ttu-id="7479b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7479b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7479b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7479b-122">JSON Representation</span></span>
<span data-ttu-id="7479b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7479b-123">Here is a JSON representation of the resource.</span></span>
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





