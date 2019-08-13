---
title: tipo de recurso macOSLobChildApp
description: Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b665391a4e7832feea72302db9ffb49c98f69964
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365913"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="dd15e-103">tipo de recurso macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="dd15e-103">macOSLobChildApp resource type</span></span>

> <span data-ttu-id="dd15e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dd15e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd15e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dd15e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd15e-106">Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="dd15e-106">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="dd15e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd15e-107">Properties</span></span>
|<span data-ttu-id="dd15e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd15e-108">Property</span></span>|<span data-ttu-id="dd15e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd15e-109">Type</span></span>|<span data-ttu-id="dd15e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd15e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd15e-111">bundleId</span><span class="sxs-lookup"><span data-stu-id="dd15e-111">bundleId</span></span>|<span data-ttu-id="dd15e-112">String</span><span class="sxs-lookup"><span data-stu-id="dd15e-112">String</span></span>|<span data-ttu-id="dd15e-113">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="dd15e-113">The Identity Name.</span></span>|
|<span data-ttu-id="dd15e-114">buildNumber</span><span class="sxs-lookup"><span data-stu-id="dd15e-114">buildNumber</span></span>|<span data-ttu-id="dd15e-115">String</span><span class="sxs-lookup"><span data-stu-id="dd15e-115">String</span></span>|<span data-ttu-id="dd15e-116">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="dd15e-116">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="dd15e-117">versionNumber</span><span class="sxs-lookup"><span data-stu-id="dd15e-117">versionNumber</span></span>|<span data-ttu-id="dd15e-118">String</span><span class="sxs-lookup"><span data-stu-id="dd15e-118">String</span></span>|<span data-ttu-id="dd15e-119">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="dd15e-119">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd15e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="dd15e-120">Relationships</span></span>
<span data-ttu-id="dd15e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd15e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd15e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd15e-122">JSON Representation</span></span>
<span data-ttu-id="dd15e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd15e-123">Here is a JSON representation of the resource.</span></span>
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



