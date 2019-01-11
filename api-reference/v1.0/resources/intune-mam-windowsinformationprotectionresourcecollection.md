---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0df0ebc3c67e7cf9bc18240f75d620442f80e0d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844349"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="ea1c3-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="ea1c3-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="ea1c3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ea1c3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea1c3-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="ea1c3-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="ea1c3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea1c3-106">Properties</span></span>
|<span data-ttu-id="ea1c3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea1c3-107">Property</span></span>|<span data-ttu-id="ea1c3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea1c3-108">Type</span></span>|<span data-ttu-id="ea1c3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea1c3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea1c3-110">displayName</span><span class="sxs-lookup"><span data-stu-id="ea1c3-110">displayName</span></span>|<span data-ttu-id="ea1c3-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea1c3-111">String</span></span>|<span data-ttu-id="ea1c3-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="ea1c3-112">Display name</span></span>|
|<span data-ttu-id="ea1c3-113">recursos</span><span class="sxs-lookup"><span data-stu-id="ea1c3-113">resources</span></span>|<span data-ttu-id="ea1c3-114">String collection</span><span class="sxs-lookup"><span data-stu-id="ea1c3-114">String collection</span></span>|<span data-ttu-id="ea1c3-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="ea1c3-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea1c3-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ea1c3-116">Relationships</span></span>
<span data-ttu-id="ea1c3-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea1c3-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea1c3-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea1c3-118">JSON Representation</span></span>
<span data-ttu-id="ea1c3-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea1c3-119">Here is a JSON representation of the resource.</span></span>
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



