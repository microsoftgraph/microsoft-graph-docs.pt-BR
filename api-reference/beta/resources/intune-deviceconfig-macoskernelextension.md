---
title: tipo de recurso macOSKernelExtension
description: Representa uma extensão de kernel macOS específica. Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22d37a87a8cdc33791907d305eca36d8ceb0fb8c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701470"
---
# <a name="macoskernelextension-resource-type"></a><span data-ttu-id="77091-104">tipo de recurso macOSKernelExtension</span><span class="sxs-lookup"><span data-stu-id="77091-104">macOSKernelExtension resource type</span></span>

<span data-ttu-id="77091-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77091-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77091-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="77091-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="77091-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="77091-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77091-108">Representa uma extensão de kernel macOS específica.</span><span class="sxs-lookup"><span data-stu-id="77091-108">Represents a specific macOS kernel extension.</span></span> <span data-ttu-id="77091-109">Uma extensão de kernel macOS pode ser descrita por seu identificador de equipe e seu identificador de pacote.</span><span class="sxs-lookup"><span data-stu-id="77091-109">A macOS kernel extension can be described by its team identifier plus its bundle identifier.</span></span>

## <a name="properties"></a><span data-ttu-id="77091-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="77091-110">Properties</span></span>
|<span data-ttu-id="77091-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77091-111">Property</span></span>|<span data-ttu-id="77091-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="77091-112">Type</span></span>|<span data-ttu-id="77091-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="77091-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77091-114">teamIdentifier</span><span class="sxs-lookup"><span data-stu-id="77091-114">teamIdentifier</span></span>|<span data-ttu-id="77091-115">String</span><span class="sxs-lookup"><span data-stu-id="77091-115">String</span></span>|<span data-ttu-id="77091-116">O identificador de equipe que foi usado para assinar a extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="77091-116">The team identifier that was used to sign the kernel extension.</span></span>|
|<span data-ttu-id="77091-117">bundleId</span><span class="sxs-lookup"><span data-stu-id="77091-117">bundleId</span></span>|<span data-ttu-id="77091-118">String</span><span class="sxs-lookup"><span data-stu-id="77091-118">String</span></span>|<span data-ttu-id="77091-119">ID do pacote da extensão do kernel.</span><span class="sxs-lookup"><span data-stu-id="77091-119">Bundle ID of the kernel extension.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77091-120">Relações</span><span class="sxs-lookup"><span data-stu-id="77091-120">Relationships</span></span>
<span data-ttu-id="77091-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="77091-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77091-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="77091-122">JSON Representation</span></span>
<span data-ttu-id="77091-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="77091-123">Here is a JSON representation of the resource.</span></span>
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





