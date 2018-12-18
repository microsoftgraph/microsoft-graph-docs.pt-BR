---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
ms.openlocfilehash: 8e037ff53e11566aee7d79d2c3bbe5b1075b83a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327829"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="a5746-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="a5746-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="a5746-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a5746-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a5746-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="a5746-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="a5746-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a5746-106">Properties</span></span>
|<span data-ttu-id="a5746-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a5746-107">Property</span></span>|<span data-ttu-id="a5746-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a5746-108">Type</span></span>|<span data-ttu-id="a5746-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a5746-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5746-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a5746-110">displayName</span></span>|<span data-ttu-id="a5746-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a5746-111">String</span></span>|<span data-ttu-id="a5746-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="a5746-112">Display name</span></span>|
|<span data-ttu-id="a5746-113">recursos</span><span class="sxs-lookup"><span data-stu-id="a5746-113">resources</span></span>|<span data-ttu-id="a5746-114">String collection</span><span class="sxs-lookup"><span data-stu-id="a5746-114">String collection</span></span>|<span data-ttu-id="a5746-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="a5746-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="a5746-116">Relações</span><span class="sxs-lookup"><span data-stu-id="a5746-116">Relationships</span></span>
<span data-ttu-id="a5746-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a5746-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a5746-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a5746-118">JSON Representation</span></span>
<span data-ttu-id="a5746-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a5746-119">Here is a JSON representation of the resource.</span></span>
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



