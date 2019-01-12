---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a913f90c2fed24a524e07b8dca1b629ebd9795f6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981214"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="cc82f-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="cc82f-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="cc82f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cc82f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc82f-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="cc82f-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="cc82f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cc82f-106">Properties</span></span>
|<span data-ttu-id="cc82f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cc82f-107">Property</span></span>|<span data-ttu-id="cc82f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cc82f-108">Type</span></span>|<span data-ttu-id="cc82f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cc82f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc82f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="cc82f-110">displayName</span></span>|<span data-ttu-id="cc82f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cc82f-111">String</span></span>|<span data-ttu-id="cc82f-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="cc82f-112">Display name</span></span>|
|<span data-ttu-id="cc82f-113">recursos</span><span class="sxs-lookup"><span data-stu-id="cc82f-113">resources</span></span>|<span data-ttu-id="cc82f-114">String collection</span><span class="sxs-lookup"><span data-stu-id="cc82f-114">String collection</span></span>|<span data-ttu-id="cc82f-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="cc82f-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc82f-116">Relações</span><span class="sxs-lookup"><span data-stu-id="cc82f-116">Relationships</span></span>
<span data-ttu-id="cc82f-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cc82f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc82f-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cc82f-118">JSON Representation</span></span>
<span data-ttu-id="cc82f-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cc82f-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```



