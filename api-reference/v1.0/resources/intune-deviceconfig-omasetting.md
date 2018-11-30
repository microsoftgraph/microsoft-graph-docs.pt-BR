---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
ms.openlocfilehash: 7ef8617ca4ce10ebeabf0d7a4655688e58925646
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004820"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="b1b16-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="b1b16-103">omaSetting resource type</span></span>

> <span data-ttu-id="b1b16-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b1b16-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b1b16-105">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b1b16-105">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="b1b16-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1b16-106">Properties</span></span>
|<span data-ttu-id="b1b16-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1b16-107">Property</span></span>|<span data-ttu-id="b1b16-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1b16-108">Type</span></span>|<span data-ttu-id="b1b16-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1b16-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1b16-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b1b16-110">displayName</span></span>|<span data-ttu-id="b1b16-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1b16-111">String</span></span>|<span data-ttu-id="b1b16-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b1b16-112">Display Name.</span></span>|
|<span data-ttu-id="b1b16-113">descrição</span><span class="sxs-lookup"><span data-stu-id="b1b16-113">description</span></span>|<span data-ttu-id="b1b16-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1b16-114">String</span></span>|<span data-ttu-id="b1b16-115">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b1b16-115">Description.</span></span>|
|<span data-ttu-id="b1b16-116">omaUri</span><span class="sxs-lookup"><span data-stu-id="b1b16-116">omaUri</span></span>|<span data-ttu-id="b1b16-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b1b16-117">String</span></span>|<span data-ttu-id="b1b16-118">OMA.</span><span class="sxs-lookup"><span data-stu-id="b1b16-118">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1b16-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b1b16-119">Relationships</span></span>
<span data-ttu-id="b1b16-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1b16-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b1b16-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1b16-121">JSON Representation</span></span>
<span data-ttu-id="b1b16-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1b16-122">Here is a JSON representation of the resource.</span></span>
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



