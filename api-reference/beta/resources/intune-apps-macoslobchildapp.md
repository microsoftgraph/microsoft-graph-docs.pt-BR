---
title: tipo de recurso macOSLobChildApp
description: Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ba9dcf62c94d316f404a56c71165357aa3c35a1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731999"
---
# <a name="macoslobchildapp-resource-type"></a><span data-ttu-id="befdb-103">tipo de recurso macOSLobChildApp</span><span class="sxs-lookup"><span data-stu-id="befdb-103">macOSLobChildApp resource type</span></span>

<span data-ttu-id="befdb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="befdb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="befdb-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="befdb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="befdb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="befdb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="befdb-107">Contém as propriedades do aplicativo de LOB do MacOS em um pacote de pacote</span><span class="sxs-lookup"><span data-stu-id="befdb-107">Contains properties the MacOS LOB App in a bundle package</span></span>

## <a name="properties"></a><span data-ttu-id="befdb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="befdb-108">Properties</span></span>
|<span data-ttu-id="befdb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="befdb-109">Property</span></span>|<span data-ttu-id="befdb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="befdb-110">Type</span></span>|<span data-ttu-id="befdb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="befdb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="befdb-112">bundleId</span><span class="sxs-lookup"><span data-stu-id="befdb-112">bundleId</span></span>|<span data-ttu-id="befdb-113">String</span><span class="sxs-lookup"><span data-stu-id="befdb-113">String</span></span>|<span data-ttu-id="befdb-114">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="befdb-114">The Identity Name.</span></span>|
|<span data-ttu-id="befdb-115">buildNumber</span><span class="sxs-lookup"><span data-stu-id="befdb-115">buildNumber</span></span>|<span data-ttu-id="befdb-116">String</span><span class="sxs-lookup"><span data-stu-id="befdb-116">String</span></span>|<span data-ttu-id="befdb-117">O número de compilação do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="befdb-117">The build number of MacOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="befdb-118">versionNumber</span><span class="sxs-lookup"><span data-stu-id="befdb-118">versionNumber</span></span>|<span data-ttu-id="befdb-119">String</span><span class="sxs-lookup"><span data-stu-id="befdb-119">String</span></span>|<span data-ttu-id="befdb-120">O número da versão do aplicativo de linha de negócios (LoB) MacOS.</span><span class="sxs-lookup"><span data-stu-id="befdb-120">The version number of MacOS Line of Business (LoB) app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="befdb-121">Relações</span><span class="sxs-lookup"><span data-stu-id="befdb-121">Relationships</span></span>
<span data-ttu-id="befdb-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="befdb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="befdb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="befdb-123">JSON Representation</span></span>
<span data-ttu-id="befdb-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="befdb-124">Here is a JSON representation of the resource.</span></span>
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





