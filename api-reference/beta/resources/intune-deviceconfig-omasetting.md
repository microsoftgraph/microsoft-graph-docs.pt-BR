---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e6cb37078eb6c5b4aee00a9ac7bfc77061ec0bcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946592"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="dc7e4-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="dc7e4-103">omaSetting resource type</span></span>

> <span data-ttu-id="dc7e4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dc7e4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dc7e4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc7e4-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="dc7e4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc7e4-108">Properties</span></span>
|<span data-ttu-id="dc7e4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc7e4-109">Property</span></span>|<span data-ttu-id="dc7e4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc7e4-110">Type</span></span>|<span data-ttu-id="dc7e4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc7e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc7e4-112">displayName</span><span class="sxs-lookup"><span data-stu-id="dc7e4-112">displayName</span></span>|<span data-ttu-id="dc7e4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc7e4-113">String</span></span>|<span data-ttu-id="dc7e4-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-114">Display Name.</span></span>|
|<span data-ttu-id="dc7e4-115">descrição</span><span class="sxs-lookup"><span data-stu-id="dc7e4-115">description</span></span>|<span data-ttu-id="dc7e4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc7e4-116">String</span></span>|<span data-ttu-id="dc7e4-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-117">Description.</span></span>|
|<span data-ttu-id="dc7e4-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="dc7e4-118">omaUri</span></span>|<span data-ttu-id="dc7e4-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc7e4-119">String</span></span>|<span data-ttu-id="dc7e4-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dc7e4-121">Relações</span><span class="sxs-lookup"><span data-stu-id="dc7e4-121">Relationships</span></span>
<span data-ttu-id="dc7e4-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dc7e4-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dc7e4-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc7e4-123">JSON Representation</span></span>
<span data-ttu-id="dc7e4-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc7e4-124">Here is a JSON representation of the resource.</span></span>
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





