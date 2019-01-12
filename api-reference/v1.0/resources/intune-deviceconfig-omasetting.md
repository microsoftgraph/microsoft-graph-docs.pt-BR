---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 42b6d5fcea7b3b46acf8d0a119213f679d99aed6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961481"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="23c17-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="23c17-103">omaSetting resource type</span></span>

> <span data-ttu-id="23c17-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="23c17-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23c17-105">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="23c17-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="23c17-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23c17-106">Properties</span></span>
|<span data-ttu-id="23c17-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23c17-107">Property</span></span>|<span data-ttu-id="23c17-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="23c17-108">Type</span></span>|<span data-ttu-id="23c17-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="23c17-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23c17-110">displayName</span><span class="sxs-lookup"><span data-stu-id="23c17-110">displayName</span></span>|<span data-ttu-id="23c17-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23c17-111">String</span></span>|<span data-ttu-id="23c17-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="23c17-112">Display Name.</span></span>|
|<span data-ttu-id="23c17-113">descrição</span><span class="sxs-lookup"><span data-stu-id="23c17-113">description</span></span>|<span data-ttu-id="23c17-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23c17-114">String</span></span>|<span data-ttu-id="23c17-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="23c17-115">Description.</span></span>|
|<span data-ttu-id="23c17-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="23c17-116">omaUri</span></span>|<span data-ttu-id="23c17-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="23c17-117">String</span></span>|<span data-ttu-id="23c17-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="23c17-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23c17-119">Relações</span><span class="sxs-lookup"><span data-stu-id="23c17-119">Relationships</span></span>
<span data-ttu-id="23c17-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23c17-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23c17-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23c17-121">JSON Representation</span></span>
<span data-ttu-id="23c17-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23c17-122">Here is a JSON representation of the resource.</span></span>
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



