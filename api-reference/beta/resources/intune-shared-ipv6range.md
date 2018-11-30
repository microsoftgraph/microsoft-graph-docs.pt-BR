---
title: Tipo de recurso iPv6Range
description: Intervalo de IPV6
ms.openlocfilehash: ac2834ea68e1ce4aa7e28f7b421ff4e3d031f8fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040876"
---
# <a name="ipv6range-resource-type"></a><span data-ttu-id="987df-103">Tipo de recurso iPv6Range</span><span class="sxs-lookup"><span data-stu-id="987df-103">iPv6Range resource type</span></span>

> <span data-ttu-id="987df-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="987df-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="987df-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="987df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="987df-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="987df-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="987df-107">Intervalo de IPV6</span><span class="sxs-lookup"><span data-stu-id="987df-107">IP V6 range</span></span>

<span data-ttu-id="987df-108">Herda de [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="987df-108">Inherits from [ipRange](../resources/intune-shared-iprange.md)</span></span>

## <a name="properties"></a><span data-ttu-id="987df-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="987df-109">Properties</span></span>
|<span data-ttu-id="987df-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="987df-110">Property</span></span>|<span data-ttu-id="987df-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="987df-111">Type</span></span>|<span data-ttu-id="987df-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="987df-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="987df-113">lowerAddress</span><span class="sxs-lookup"><span data-stu-id="987df-113">lowerAddress</span></span>|<span data-ttu-id="987df-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="987df-114">String</span></span>|<span data-ttu-id="987df-115">Endereço IP de número mais baixo</span><span class="sxs-lookup"><span data-stu-id="987df-115">Lower IP Address</span></span>|
|<span data-ttu-id="987df-116">upperAddress</span><span class="sxs-lookup"><span data-stu-id="987df-116">upperAddress</span></span>|<span data-ttu-id="987df-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="987df-117">String</span></span>|<span data-ttu-id="987df-118">Endereço IP de número mais alto</span><span class="sxs-lookup"><span data-stu-id="987df-118">Upper IP Address</span></span>|

## <a name="relationships"></a><span data-ttu-id="987df-119">Relações</span><span class="sxs-lookup"><span data-stu-id="987df-119">Relationships</span></span>
<span data-ttu-id="987df-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="987df-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="987df-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="987df-121">JSON Representation</span></span>
<span data-ttu-id="987df-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="987df-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iPv6Range"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iPv6Range",
  "lowerAddress": "String",
  "upperAddress": "String"
}
```



