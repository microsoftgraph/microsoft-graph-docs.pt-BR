---
title: tipo de recurso iosAvailableUpdateVersion
description: detalhes da versão da atualização disponível do iOS
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2113f8ddf34c87be6554bc29d7220881e8c634f6
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160786"
---
# <a name="iosavailableupdateversion-resource-type"></a><span data-ttu-id="d9d6c-103">tipo de recurso iosAvailableUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="d9d6c-103">iosAvailableUpdateVersion resource type</span></span>

> <span data-ttu-id="d9d6c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9d6c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9d6c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9d6c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9d6c-106">detalhes da versão da atualização disponível do iOS</span><span class="sxs-lookup"><span data-stu-id="d9d6c-106">iOS available update version details</span></span>

## <a name="properties"></a><span data-ttu-id="d9d6c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9d6c-107">Properties</span></span>
|<span data-ttu-id="d9d6c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9d6c-108">Property</span></span>|<span data-ttu-id="d9d6c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9d6c-109">Type</span></span>|<span data-ttu-id="d9d6c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9d6c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9d6c-111">productVersion</span><span class="sxs-lookup"><span data-stu-id="d9d6c-111">productVersion</span></span>|<span data-ttu-id="d9d6c-112">String</span><span class="sxs-lookup"><span data-stu-id="d9d6c-112">String</span></span>|<span data-ttu-id="d9d6c-113">A versão da atualização.</span><span class="sxs-lookup"><span data-stu-id="d9d6c-113">The version of the update.</span></span>|
|<span data-ttu-id="d9d6c-114">postingDateTime</span><span class="sxs-lookup"><span data-stu-id="d9d6c-114">postingDateTime</span></span>|<span data-ttu-id="d9d6c-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9d6c-115">DateTimeOffset</span></span>|<span data-ttu-id="d9d6c-116">A data de lançamento da atualização.</span><span class="sxs-lookup"><span data-stu-id="d9d6c-116">The posting date of the update.</span></span>|
|<span data-ttu-id="d9d6c-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d9d6c-117">expirationDateTime</span></span>|<span data-ttu-id="d9d6c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9d6c-118">DateTimeOffset</span></span>|<span data-ttu-id="d9d6c-119">A data de expiração da atualização.</span><span class="sxs-lookup"><span data-stu-id="d9d6c-119">The expiration date of the update.</span></span>|
|<span data-ttu-id="d9d6c-120">supportedDevices</span><span class="sxs-lookup"><span data-stu-id="d9d6c-120">supportedDevices</span></span>|<span data-ttu-id="d9d6c-121">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9d6c-121">String collection</span></span>|<span data-ttu-id="d9d6c-122">Lista de dispositivos com suporte para a atualização.</span><span class="sxs-lookup"><span data-stu-id="d9d6c-122">List of supported devices for the update.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9d6c-123">Relações</span><span class="sxs-lookup"><span data-stu-id="d9d6c-123">Relationships</span></span>
<span data-ttu-id="d9d6c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9d6c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9d6c-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9d6c-125">JSON Representation</span></span>
<span data-ttu-id="d9d6c-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9d6c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosAvailableUpdateVersion"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosAvailableUpdateVersion",
  "productVersion": "String",
  "postingDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "supportedDevices": [
    "String"
  ]
}
```



