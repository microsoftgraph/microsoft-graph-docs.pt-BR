---
title: tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04320f92045ae128ca1bf128484d2aa55f03d706
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808850"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="7691d-104">tipo de recurso macOSKernelExtension</span><span class="sxs-lookup"><span data-stu-id="7691d-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="7691d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7691d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7691d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7691d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7691d-107">Representa uma extensão de kernel macOS específica.</span><span class="sxs-lookup"><span data-stu-id="7691d-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="7691d-108">Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.</span><span class="sxs-lookup"><span data-stu-id="7691d-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="7691d-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7691d-109">Properties</span></span>
|<span data-ttu-id="7691d-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7691d-110">Property</span></span>|<span data-ttu-id="7691d-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="7691d-111">Type</span></span>|<span data-ttu-id="7691d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="7691d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7691d-113">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="7691d-113">teamIdentifier</span></span>|<span data-ttu-id="7691d-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7691d-114">String</span></span>|<span data-ttu-id="7691d-115">O identificador de equipe que foi usado para assinar a extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="7691d-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="7691d-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="7691d-116">bundleId</span></span>|<span data-ttu-id="7691d-117">String</span><span class="sxs-lookup"><span data-stu-id="7691d-117">String</span></span>|<span data-ttu-id="7691d-118">ID do pacote da extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="7691d-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7691d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7691d-119">Relationships</span></span>
<span data-ttu-id="7691d-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7691d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7691d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7691d-121">JSON Representation</span></span>
<span data-ttu-id="7691d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7691d-122">Here is a JSON representation of the resource.</span></span>
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





