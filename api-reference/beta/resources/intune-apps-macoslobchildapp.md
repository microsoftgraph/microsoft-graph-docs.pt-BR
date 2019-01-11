---
title: tipo de recurso de macOSLobChildApp
description: Contém propriedades o MacOS LOB App em um pacote de pacote
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2fd4440422ee184b62da4731f49ead4316a2fa45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851244"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="45dfd-103">tipo de recurso de macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="45dfd-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="45dfd-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="45dfd-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45dfd-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="45dfd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45dfd-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="45dfd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45dfd-107">Contém propriedades o MacOS LOB App em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="45dfd-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="45dfd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="45dfd-108">Properties</span></span>
|<span data-ttu-id="45dfd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="45dfd-109">Property</span></span>|<span data-ttu-id="45dfd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="45dfd-110">Type</span></span>|<span data-ttu-id="45dfd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="45dfd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45dfd-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="45dfd-112">bundleId</span></span>|<span data-ttu-id="45dfd-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45dfd-113">String</span></span>|<span data-ttu-id="45dfd-114">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="45dfd-114">The Identity Name.</span></span>|
|<span data-ttu-id="45dfd-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="45dfd-115">buildNumber</span></span>|<span data-ttu-id="45dfd-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45dfd-116">String</span></span>|<span data-ttu-id="45dfd-117">O número de compilação da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="45dfd-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="45dfd-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="45dfd-118">versionNumber</span></span>|<span data-ttu-id="45dfd-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="45dfd-119">String</span></span>|<span data-ttu-id="45dfd-120">O número de versão da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="45dfd-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45dfd-121">Relações</span><span class="sxs-lookup"><span data-stu-id="45dfd-121">Relationships</span></span>
<span data-ttu-id="45dfd-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="45dfd-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="45dfd-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="45dfd-123">JSON Representation</span></span>
<span data-ttu-id="45dfd-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="45dfd-124">Here is a JSON representation of the resource.</span></span>
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





