---
title: Tipo de recurso omaSetting
description: Configurações de OMA.
ms.openlocfilehash: 900e3f4d8e24743ed75b15f7a57188b46630c9fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034399"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="b27d9-103">Tipo de recurso omaSetting</span><span class="sxs-lookup"><span data-stu-id="b27d9-103">omaSetting resource type</span></span>

> <span data-ttu-id="b27d9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b27d9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b27d9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b27d9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b27d9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b27d9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b27d9-107">Configurações de OMA.</span><span class="sxs-lookup"><span data-stu-id="b27d9-107">OMA Settings definition.</span></span>
## <a name="properties"></a><span data-ttu-id="b27d9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b27d9-108">Properties</span></span>
|<span data-ttu-id="b27d9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b27d9-109">Property</span></span>|<span data-ttu-id="b27d9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b27d9-110">Type</span></span>|<span data-ttu-id="b27d9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b27d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b27d9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b27d9-112">displayName</span></span>|<span data-ttu-id="b27d9-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b27d9-113">String</span></span>|<span data-ttu-id="b27d9-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="b27d9-114">Display Name.</span></span>|
|<span data-ttu-id="b27d9-115">descrição</span><span class="sxs-lookup"><span data-stu-id="b27d9-115">description</span></span>|<span data-ttu-id="b27d9-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b27d9-116">String</span></span>|<span data-ttu-id="b27d9-117">Descrição.</span><span class="sxs-lookup"><span data-stu-id="b27d9-117">Description.</span></span>|
|<span data-ttu-id="b27d9-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="b27d9-118">omaUri</span></span>|<span data-ttu-id="b27d9-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b27d9-119">String</span></span>|<span data-ttu-id="b27d9-120">OMA.</span><span class="sxs-lookup"><span data-stu-id="b27d9-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b27d9-121">Relações</span><span class="sxs-lookup"><span data-stu-id="b27d9-121">Relationships</span></span>
<span data-ttu-id="b27d9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b27d9-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b27d9-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b27d9-123">JSON Representation</span></span>
<span data-ttu-id="b27d9-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b27d9-124">Here is a JSON representation of the resource.</span></span>
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





