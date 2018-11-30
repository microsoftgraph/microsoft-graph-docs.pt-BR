---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
ms.openlocfilehash: fd350f85acb962267f92352e6298dc50c44949ed
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005098"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="2fc39-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="2fc39-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="2fc39-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2fc39-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fc39-105">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="2fc39-105">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="2fc39-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fc39-106">Properties</span></span>
|<span data-ttu-id="2fc39-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fc39-107">Property</span></span>|<span data-ttu-id="2fc39-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fc39-108">Type</span></span>|<span data-ttu-id="2fc39-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fc39-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fc39-110">displayName</span><span class="sxs-lookup"><span data-stu-id="2fc39-110">displayName</span></span>|<span data-ttu-id="2fc39-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2fc39-111">String</span></span>|<span data-ttu-id="2fc39-112">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="2fc39-112">Display name</span></span>|
|<span data-ttu-id="2fc39-113">recursos</span><span class="sxs-lookup"><span data-stu-id="2fc39-113">resources</span></span>|<span data-ttu-id="2fc39-114">String collection</span><span class="sxs-lookup"><span data-stu-id="2fc39-114">String collection</span></span>|<span data-ttu-id="2fc39-115">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="2fc39-115">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fc39-116">Relações</span><span class="sxs-lookup"><span data-stu-id="2fc39-116">Relationships</span></span>
<span data-ttu-id="2fc39-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fc39-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2fc39-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fc39-118">JSON Representation</span></span>
<span data-ttu-id="2fc39-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fc39-119">Here is a JSON representation of the resource.</span></span>
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



