---
title: tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca91021ccb9fbc4cf8ec6c61b4edea979bb7c833
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523200"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="db701-103">tipo de recurso synchronizationJobApplicationParameters</span><span class="sxs-lookup"><span data-stu-id="db701-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="db701-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="db701-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="db701-105">Representa os objetos que serão provisionados e as regras de sincronização executadas.</span><span class="sxs-lookup"><span data-stu-id="db701-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="db701-106">O recurso é usado principalmente para provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="db701-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="db701-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db701-107">Properties</span></span>
|<span data-ttu-id="db701-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db701-108">Property</span></span>|<span data-ttu-id="db701-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="db701-109">Type</span></span>|<span data-ttu-id="db701-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db701-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db701-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="db701-111">ruleId</span></span>|<span data-ttu-id="db701-112">String</span><span class="sxs-lookup"><span data-stu-id="db701-112">String</span></span>|<span data-ttu-id="db701-113">O identificador de um synchronizationRule a ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="db701-113">The identifier of a the synchronizationRule to be applied.</span></span>|
|<span data-ttu-id="db701-114">olhos</span><span class="sxs-lookup"><span data-stu-id="db701-114">subjects</span></span>|<span data-ttu-id="db701-115">coleção [synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)</span><span class="sxs-lookup"><span data-stu-id="db701-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="db701-116">Os identificadores de um ou mais objetos aos quais um synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="db701-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db701-117">Relações</span><span class="sxs-lookup"><span data-stu-id="db701-117">Relationships</span></span>
<span data-ttu-id="db701-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db701-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="db701-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db701-119">JSON representation</span></span>
<span data-ttu-id="db701-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db701-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobApplicationParameters"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobApplicationParameters",
  "ruleId": "String",
  "subjects": [
    {
      "@odata.type": "microsoft.graph.synchronizationJobSubject"
    }
  ]
}
```


