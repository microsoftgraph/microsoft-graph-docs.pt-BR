---
title: tipo de recurso de macOSLobChildApp
description: Contém propriedades o MacOS LOB App em um pacote de pacote
ms.openlocfilehash: 6035e77843923eacbce8a1647de241fc79338766
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036562"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="47f79-103">tipo de recurso de macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="47f79-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="47f79-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="47f79-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47f79-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="47f79-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="47f79-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="47f79-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="47f79-107">Contém propriedades o MacOS LOB App em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="47f79-107">Contains properties the MacOS LOB App in a bundle package</span></span>
## <a name="properties"></a><span data-ttu-id="47f79-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47f79-108">Properties</span></span>
|<span data-ttu-id="47f79-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47f79-109">Property</span></span>|<span data-ttu-id="47f79-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="47f79-110">Type</span></span>|<span data-ttu-id="47f79-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="47f79-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47f79-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="47f79-112">bundleId</span></span>|<span data-ttu-id="47f79-113">String</span><span class="sxs-lookup"><span data-stu-id="47f79-113">String</span></span>|<span data-ttu-id="47f79-114">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="47f79-114">The Identity Name.</span></span>|
|<span data-ttu-id="47f79-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="47f79-115">buildNumber</span></span>|<span data-ttu-id="47f79-116">String</span><span class="sxs-lookup"><span data-stu-id="47f79-116">String</span></span>|<span data-ttu-id="47f79-117">O número de compilação da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="47f79-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="47f79-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="47f79-118">versionNumber</span></span>|<span data-ttu-id="47f79-119">String</span><span class="sxs-lookup"><span data-stu-id="47f79-119">String</span></span>|<span data-ttu-id="47f79-120">O número de versão da linha de MacOS do aplicativo de negócios (LoB).</span><span class="sxs-lookup"><span data-stu-id="47f79-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="47f79-121">Relações</span><span class="sxs-lookup"><span data-stu-id="47f79-121">Relationships</span></span>
<span data-ttu-id="47f79-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47f79-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="47f79-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47f79-123">JSON Representation</span></span>
<span data-ttu-id="47f79-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47f79-124">Here is a JSON representation of the resource.</span></span>
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





