---
title: tipo de recurso macOSLobChildApp
description: Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b3c115e312333a448318fb718140f5b6e8305494
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49281828"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="da183-103">tipo de recurso macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="da183-103">macOSLobChildApp resource type</span></span>

<span data-ttu-id="da183-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da183-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da183-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da183-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da183-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da183-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da183-107">Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="da183-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="da183-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da183-108">Properties</span></span>
|<span data-ttu-id="da183-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da183-109">Property</span></span>|<span data-ttu-id="da183-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da183-110">Type</span></span>|<span data-ttu-id="da183-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da183-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da183-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="da183-112">bundleId</span></span>|<span data-ttu-id="da183-113">String</span><span class="sxs-lookup"><span data-stu-id="da183-113">String</span></span>|<span data-ttu-id="da183-114">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="da183-114">The Identity Name.</span></span>|
|<span data-ttu-id="da183-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="da183-115">buildNumber</span></span>|<span data-ttu-id="da183-116">String</span><span class="sxs-lookup"><span data-stu-id="da183-116">String</span></span>|<span data-ttu-id="da183-117">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="da183-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="da183-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="da183-118">versionNumber</span></span>|<span data-ttu-id="da183-119">String</span><span class="sxs-lookup"><span data-stu-id="da183-119">String</span></span>|<span data-ttu-id="da183-120">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="da183-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da183-121">Relações</span><span class="sxs-lookup"><span data-stu-id="da183-121">Relationships</span></span>
<span data-ttu-id="da183-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da183-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da183-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da183-123">JSON Representation</span></span>
<span data-ttu-id="da183-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da183-124">Here is a JSON representation of the resource.</span></span>
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




