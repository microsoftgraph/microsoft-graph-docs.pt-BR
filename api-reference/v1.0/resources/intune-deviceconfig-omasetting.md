---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: tfitzmac
ms.openlocfilehash: 564912635fbcd5e2846965d3546a3830119db252
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340884"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="1ee6e-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="1ee6e-103">omaSetting resource type</span></span>

> <span data-ttu-id="1ee6e-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1ee6e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ee6e-105">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="1ee6e-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="1ee6e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ee6e-106">Properties</span></span>
|<span data-ttu-id="1ee6e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ee6e-107">Property</span></span>|<span data-ttu-id="1ee6e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ee6e-108">Type</span></span>|<span data-ttu-id="1ee6e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ee6e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ee6e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="1ee6e-110">displayName</span></span>|<span data-ttu-id="1ee6e-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ee6e-111">String</span></span>|<span data-ttu-id="1ee6e-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1ee6e-112">Display Name.</span></span>|
|<span data-ttu-id="1ee6e-113">descrição</span><span class="sxs-lookup"><span data-stu-id="1ee6e-113">description</span></span>|<span data-ttu-id="1ee6e-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ee6e-114">String</span></span>|<span data-ttu-id="1ee6e-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="1ee6e-115">Description.</span></span>|
|<span data-ttu-id="1ee6e-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="1ee6e-116">omaUri</span></span>|<span data-ttu-id="1ee6e-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ee6e-117">String</span></span>|<span data-ttu-id="1ee6e-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="1ee6e-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ee6e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1ee6e-119">Relationships</span></span>
<span data-ttu-id="1ee6e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1ee6e-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1ee6e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ee6e-121">JSON Representation</span></span>
<span data-ttu-id="1ee6e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1ee6e-122">Here is a JSON representation of the resource.</span></span>
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



