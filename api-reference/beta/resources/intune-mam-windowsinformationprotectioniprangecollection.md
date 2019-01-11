---
title: Tipo de recurso windowsInformationProtectionIPRangeCollection
description: Coleção de intervalos de IP da Proteção de Informações do Windows
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 73995f6b8f5e376de53ec88772dc3713cc179f3a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838602"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="eee48-103">Tipo de recurso windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="eee48-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="eee48-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="eee48-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eee48-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="eee48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eee48-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="eee48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eee48-107">Coleção de intervalos de IP da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="eee48-107">Windows Information Protection IP Range Collection</span></span>
## <a name="properties"></a><span data-ttu-id="eee48-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eee48-108">Properties</span></span>
|<span data-ttu-id="eee48-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eee48-109">Property</span></span>|<span data-ttu-id="eee48-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="eee48-110">Type</span></span>|<span data-ttu-id="eee48-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="eee48-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eee48-112">displayName</span><span class="sxs-lookup"><span data-stu-id="eee48-112">displayName</span></span>|<span data-ttu-id="eee48-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eee48-113">String</span></span>|<span data-ttu-id="eee48-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="eee48-114">Display name</span></span>|
|<span data-ttu-id="eee48-115">ranges</span><span class="sxs-lookup"><span data-stu-id="eee48-115">ranges</span></span>|<span data-ttu-id="eee48-116">Coleção [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="eee48-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="eee48-117">Coleção de intervalos de IP</span><span class="sxs-lookup"><span data-stu-id="eee48-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="eee48-118">Relações</span><span class="sxs-lookup"><span data-stu-id="eee48-118">Relationships</span></span>
<span data-ttu-id="eee48-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eee48-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eee48-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eee48-120">JSON Representation</span></span>
<span data-ttu-id="eee48-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eee48-121">Here is a JSON representation of the resource.</span></span>
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





