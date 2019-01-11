---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 86cb06b35a0f64052860c268764696a1db8459e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888379"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="d1306-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="d1306-103">omaSetting resource type</span></span>

> <span data-ttu-id="d1306-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d1306-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1306-105">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="d1306-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="d1306-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d1306-106">Properties</span></span>
|<span data-ttu-id="d1306-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d1306-107">Property</span></span>|<span data-ttu-id="d1306-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d1306-108">Type</span></span>|<span data-ttu-id="d1306-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d1306-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1306-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d1306-110">displayName</span></span>|<span data-ttu-id="d1306-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1306-111">String</span></span>|<span data-ttu-id="d1306-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="d1306-112">Display Name.</span></span>|
|<span data-ttu-id="d1306-113">descrição</span><span class="sxs-lookup"><span data-stu-id="d1306-113">description</span></span>|<span data-ttu-id="d1306-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1306-114">String</span></span>|<span data-ttu-id="d1306-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="d1306-115">Description.</span></span>|
|<span data-ttu-id="d1306-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="d1306-116">omaUri</span></span>|<span data-ttu-id="d1306-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d1306-117">String</span></span>|<span data-ttu-id="d1306-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="d1306-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1306-119">Relações</span><span class="sxs-lookup"><span data-stu-id="d1306-119">Relationships</span></span>
<span data-ttu-id="d1306-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d1306-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1306-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d1306-121">JSON Representation</span></span>
<span data-ttu-id="d1306-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d1306-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```



