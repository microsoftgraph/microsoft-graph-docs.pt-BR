---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
author: tfitzmac
ms.openlocfilehash: 96b3b36f40d1eeb88731f6f44ebec812a18fe713
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306885"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="5f906-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="5f906-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="5f906-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5f906-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f906-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5f906-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5f906-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="5f906-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f906-107">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="5f906-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="5f906-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5f906-108">Properties</span></span>
|<span data-ttu-id="5f906-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5f906-109">Property</span></span>|<span data-ttu-id="5f906-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5f906-110">Type</span></span>|<span data-ttu-id="5f906-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5f906-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f906-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5f906-112">displayName</span></span>|<span data-ttu-id="5f906-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5f906-113">String</span></span>|<span data-ttu-id="5f906-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="5f906-114">Display name</span></span>|
|<span data-ttu-id="5f906-115">recursos</span><span class="sxs-lookup"><span data-stu-id="5f906-115">resources</span></span>|<span data-ttu-id="5f906-116">String collection</span><span class="sxs-lookup"><span data-stu-id="5f906-116">String collection</span></span>|<span data-ttu-id="5f906-117">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="5f906-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f906-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5f906-118">Relationships</span></span>
<span data-ttu-id="5f906-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5f906-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5f906-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5f906-120">JSON Representation</span></span>
<span data-ttu-id="5f906-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5f906-121">Here is a JSON representation of the resource.</span></span>
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





