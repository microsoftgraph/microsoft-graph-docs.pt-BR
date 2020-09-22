---
title: tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: eaa569faa7705baf95ef5843ad0ae1e66a0bf1ff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026107"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="3ba0f-103">tipo de recurso synchronizationJobApplicationParameters</span><span class="sxs-lookup"><span data-stu-id="3ba0f-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="3ba0f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ba0f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3ba0f-105">Representa os objetos que serão provisionados e as regras de sincronização executadas.</span><span class="sxs-lookup"><span data-stu-id="3ba0f-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="3ba0f-106">O recurso é usado principalmente para provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="3ba0f-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="3ba0f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ba0f-107">Properties</span></span>
|<span data-ttu-id="3ba0f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ba0f-108">Property</span></span>|<span data-ttu-id="3ba0f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ba0f-109">Type</span></span>|<span data-ttu-id="3ba0f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ba0f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ba0f-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="3ba0f-111">ruleId</span></span>|<span data-ttu-id="3ba0f-112">String</span><span class="sxs-lookup"><span data-stu-id="3ba0f-112">String</span></span>|<span data-ttu-id="3ba0f-113">O identificador de um synchronizationRule a ser aplicado; opcional para um synchronizationJob com um único synchronizationRule.</span><span class="sxs-lookup"><span data-stu-id="3ba0f-113">The identifier of a the synchronizationRule to be applied; optional for a synchronizationJob with a single synchronizationRule.</span></span>|
|<span data-ttu-id="3ba0f-114">olhos</span><span class="sxs-lookup"><span data-stu-id="3ba0f-114">subjects</span></span>|<span data-ttu-id="3ba0f-115">coleção [synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)</span><span class="sxs-lookup"><span data-stu-id="3ba0f-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="3ba0f-116">Os identificadores de um ou mais objetos aos quais um synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="3ba0f-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ba0f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="3ba0f-117">Relationships</span></span>
<span data-ttu-id="3ba0f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ba0f-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ba0f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ba0f-119">JSON representation</span></span>
<span data-ttu-id="3ba0f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ba0f-120">The following is a JSON representation of the resource.</span></span>
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


