---
title: tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b75288befb0f8ba7101d88d5b6f0767174469ac3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946189"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="55550-104">tipo de recurso macOSKernelExtension</span><span class="sxs-lookup"><span data-stu-id="55550-104">macOSKernelExtension resource type</span></span>

> <span data-ttu-id="55550-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55550-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55550-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55550-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55550-107">Representa uma extensão de kernel macOS específica.</span><span class="sxs-lookup"><span data-stu-id="55550-107">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="55550-108">Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.</span><span class="sxs-lookup"><span data-stu-id="55550-108">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="55550-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55550-109">Properties</span></span>
|<span data-ttu-id="55550-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55550-110">Property</span></span>|<span data-ttu-id="55550-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="55550-111">Type</span></span>|<span data-ttu-id="55550-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="55550-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55550-113">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="55550-113">teamIdentifier</span></span>|<span data-ttu-id="55550-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55550-114">String</span></span>|<span data-ttu-id="55550-115">O identificador de equipe que foi usado para assinar a extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="55550-115">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="55550-116">bundleId</span><span class="sxs-lookup"><span data-stu-id="55550-116">bundleId</span></span>|<span data-ttu-id="55550-117">String</span><span class="sxs-lookup"><span data-stu-id="55550-117">String</span></span>|<span data-ttu-id="55550-118">ID do pacote da extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="55550-118">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55550-119">Relações</span><span class="sxs-lookup"><span data-stu-id="55550-119">Relationships</span></span>
<span data-ttu-id="55550-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55550-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55550-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55550-121">JSON Representation</span></span>
<span data-ttu-id="55550-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55550-122">Here is a JSON representation of the resource.</span></span>
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




