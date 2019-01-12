---
title: tipo de recurso de macOSLobChildApp
description: Contém propriedades o MacOS LOB App em um pacote de pacote
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43f207bb2cebccdd01c791694674c6fbf96b631f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954229"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="0a38c-103">tipo de recurso de macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="0a38c-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="0a38c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a38c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a38c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a38c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a38c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0a38c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a38c-107">Contém propriedades o MacOS LOB App em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="0a38c-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="0a38c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a38c-108">Properties</span></span>
|<span data-ttu-id="0a38c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a38c-109">Property</span></span>|<span data-ttu-id="0a38c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a38c-110">Type</span></span>|<span data-ttu-id="0a38c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a38c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a38c-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="0a38c-112">bundleId</span></span>|<span data-ttu-id="0a38c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a38c-113">String</span></span>|<span data-ttu-id="0a38c-114">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="0a38c-114">The Identity Name.</span></span>|
|<span data-ttu-id="0a38c-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="0a38c-115">buildNumber</span></span>|<span data-ttu-id="0a38c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a38c-116">String</span></span>|<span data-ttu-id="0a38c-117">O número de compilação da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="0a38c-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="0a38c-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="0a38c-118">versionNumber</span></span>|<span data-ttu-id="0a38c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0a38c-119">String</span></span>|<span data-ttu-id="0a38c-120">O número de versão da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="0a38c-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a38c-121">Relações</span><span class="sxs-lookup"><span data-stu-id="0a38c-121">Relationships</span></span>
<span data-ttu-id="0a38c-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a38c-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a38c-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a38c-123">JSON Representation</span></span>
<span data-ttu-id="0a38c-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a38c-124">Here is a JSON representation of the resource.</span></span>
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





