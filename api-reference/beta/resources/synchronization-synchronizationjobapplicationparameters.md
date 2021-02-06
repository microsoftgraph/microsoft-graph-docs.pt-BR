---
title: Tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 2c17d67f766a398f94ab4962850a762fc62f6e53
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133921"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="39ea5-103">Tipo de recurso synchronizationJobApplicationParameters</span><span class="sxs-lookup"><span data-stu-id="39ea5-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="39ea5-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39ea5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39ea5-105">Representa os objetos que serão provisionados e as regras de sincronização executadas.</span><span class="sxs-lookup"><span data-stu-id="39ea5-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="39ea5-106">O recurso é usado principalmente para provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="39ea5-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="39ea5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="39ea5-107">Properties</span></span>
|<span data-ttu-id="39ea5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="39ea5-108">Property</span></span>|<span data-ttu-id="39ea5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="39ea5-109">Type</span></span>|<span data-ttu-id="39ea5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39ea5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ea5-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="39ea5-111">ruleId</span></span>|<span data-ttu-id="39ea5-112">String</span><span class="sxs-lookup"><span data-stu-id="39ea5-112">String</span></span>|<span data-ttu-id="39ea5-113">O identificador de uma synchronizationRule a ser aplicada.</span><span class="sxs-lookup"><span data-stu-id="39ea5-113">The identifier of a the synchronizationRule to be applied.</span></span>|
|<span data-ttu-id="39ea5-114">subjects</span><span class="sxs-lookup"><span data-stu-id="39ea5-114">subjects</span></span>|<span data-ttu-id="39ea5-115">[Coleção synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)</span><span class="sxs-lookup"><span data-stu-id="39ea5-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="39ea5-116">Os identificadores de um ou mais objetos aos quais um synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="39ea5-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ea5-117">Relações</span><span class="sxs-lookup"><span data-stu-id="39ea5-117">Relationships</span></span>
<span data-ttu-id="39ea5-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="39ea5-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="39ea5-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="39ea5-119">JSON representation</span></span>
<span data-ttu-id="39ea5-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="39ea5-120">The following is a JSON representation of the resource.</span></span>
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


