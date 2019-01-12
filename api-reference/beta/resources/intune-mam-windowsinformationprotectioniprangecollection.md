---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9981b585818bb6db712b0088b2fde275179917ef
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911823"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="928dc-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="928dc-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="928dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="928dc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="928dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="928dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="928dc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="928dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="928dc-107">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="928dc-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="928dc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="928dc-108">Properties</span></span>
|<span data-ttu-id="928dc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="928dc-109">Property</span></span>|<span data-ttu-id="928dc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="928dc-110">Type</span></span>|<span data-ttu-id="928dc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="928dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="928dc-112">displayName</span><span class="sxs-lookup"><span data-stu-id="928dc-112">displayName</span></span>|<span data-ttu-id="928dc-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="928dc-113">String</span></span>|<span data-ttu-id="928dc-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="928dc-114">Display name</span></span>|
|<span data-ttu-id="928dc-115">ranges</span><span class="sxs-lookup"><span data-stu-id="928dc-115">ranges</span></span>|<span data-ttu-id="928dc-116">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="928dc-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="928dc-117">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="928dc-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="928dc-118">Relações</span><span class="sxs-lookup"><span data-stu-id="928dc-118">Relationships</span></span>
<span data-ttu-id="928dc-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="928dc-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="928dc-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="928dc-120">JSON Representation</span></span>
<span data-ttu-id="928dc-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="928dc-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```





