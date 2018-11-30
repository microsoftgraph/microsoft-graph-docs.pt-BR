---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
ms.openlocfilehash: 72b7c982197701f936a11b7b474a8acd86393260
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040119"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="04b47-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="04b47-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="04b47-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="04b47-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04b47-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="04b47-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04b47-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="04b47-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04b47-107">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="04b47-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="04b47-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04b47-108">Properties</span></span>
|<span data-ttu-id="04b47-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04b47-109">Property</span></span>|<span data-ttu-id="04b47-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04b47-110">Type</span></span>|<span data-ttu-id="04b47-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04b47-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04b47-112">displayName</span><span class="sxs-lookup"><span data-stu-id="04b47-112">displayName</span></span>|<span data-ttu-id="04b47-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="04b47-113">String</span></span>|<span data-ttu-id="04b47-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="04b47-114">Display name</span></span>|
|<span data-ttu-id="04b47-115">ranges</span><span class="sxs-lookup"><span data-stu-id="04b47-115">ranges</span></span>|<span data-ttu-id="04b47-116">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="04b47-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="04b47-117">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="04b47-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="04b47-118">Relações</span><span class="sxs-lookup"><span data-stu-id="04b47-118">Relationships</span></span>
<span data-ttu-id="04b47-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04b47-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04b47-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04b47-120">JSON Representation</span></span>
<span data-ttu-id="04b47-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04b47-121">Here is a JSON representation of the resource.</span></span>
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





