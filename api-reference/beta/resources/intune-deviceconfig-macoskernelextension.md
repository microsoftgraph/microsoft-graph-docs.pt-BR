---
title: tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 457d13b2f3f78b52457afd7c30bf3b0e36ca4e92
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43447049"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="88f67-104">tipo de recurso macOSKernelExtension</span><span class="sxs-lookup"><span data-stu-id="88f67-104">macOSKernelExtension resource type</span></span>

<span data-ttu-id="88f67-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88f67-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88f67-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="88f67-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88f67-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="88f67-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88f67-108">Representa uma extensão de kernel macOS específica.</span><span class="sxs-lookup"><span data-stu-id="88f67-108">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="88f67-109">Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.</span><span class="sxs-lookup"><span data-stu-id="88f67-109">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="88f67-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88f67-110">Properties</span></span>
|<span data-ttu-id="88f67-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88f67-111">Property</span></span>|<span data-ttu-id="88f67-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="88f67-112">Type</span></span>|<span data-ttu-id="88f67-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="88f67-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88f67-114">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="88f67-114">teamIdentifier</span></span>|<span data-ttu-id="88f67-115">String</span><span class="sxs-lookup"><span data-stu-id="88f67-115">String</span></span>|<span data-ttu-id="88f67-116">O identificador de equipe que foi usado para assinar a extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="88f67-116">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="88f67-117">bundleId</span><span class="sxs-lookup"><span data-stu-id="88f67-117">bundleId</span></span>|<span data-ttu-id="88f67-118">String</span><span class="sxs-lookup"><span data-stu-id="88f67-118">String</span></span>|<span data-ttu-id="88f67-119">ID do pacote da extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="88f67-119">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88f67-120">Relações</span><span class="sxs-lookup"><span data-stu-id="88f67-120">Relationships</span></span>
<span data-ttu-id="88f67-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88f67-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="88f67-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88f67-122">JSON Representation</span></span>
<span data-ttu-id="88f67-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88f67-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```



