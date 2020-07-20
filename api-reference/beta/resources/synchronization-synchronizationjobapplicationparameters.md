---
title: tipo de recurso synchronizationJobApplicationParameters
description: Representa os objetos a serem provisionados e as regras executadas durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: c0f0b7cae5a3ce9c49ea64b603390ea65831144b
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007139"
---
# <a name="synchronizationjobapplicationparameters-resource-type"></a><span data-ttu-id="e1302-103">tipo de recurso synchronizationJobApplicationParameters</span><span class="sxs-lookup"><span data-stu-id="e1302-103">synchronizationJobApplicationParameters resource type</span></span>

<span data-ttu-id="e1302-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1302-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e1302-105">Representa os objetos que serão provisionados e as regras de sincronização executadas.</span><span class="sxs-lookup"><span data-stu-id="e1302-105">Represents the objects that will be provisioned and the synchronization rules executed.</span></span> <span data-ttu-id="e1302-106">O recurso é usado principalmente para provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="e1302-106">The resource is primarily used for on-demand provisioning.</span></span> 

## <a name="properties"></a><span data-ttu-id="e1302-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e1302-107">Properties</span></span>
|<span data-ttu-id="e1302-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e1302-108">Property</span></span>|<span data-ttu-id="e1302-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e1302-109">Type</span></span>|<span data-ttu-id="e1302-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e1302-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1302-111">ruleId</span><span class="sxs-lookup"><span data-stu-id="e1302-111">ruleId</span></span>|<span data-ttu-id="e1302-112">String</span><span class="sxs-lookup"><span data-stu-id="e1302-112">String</span></span>|<span data-ttu-id="e1302-113">O identificador de um synchronizationRule a ser aplicado; opcional para um synchronizationJob com um único synchronizationRule.</span><span class="sxs-lookup"><span data-stu-id="e1302-113">The identifier of a the synchronizationRule to be applied; optional for a synchronizationJob with a single synchronizationRule.</span></span>|
|<span data-ttu-id="e1302-114">olhos</span><span class="sxs-lookup"><span data-stu-id="e1302-114">subjects</span></span>|<span data-ttu-id="e1302-115">coleção [synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md)</span><span class="sxs-lookup"><span data-stu-id="e1302-115">[synchronizationJobSubject](../resources/synchronization-synchronizationjobsubject.md) collection</span></span>|<span data-ttu-id="e1302-116">Os identificadores de um ou mais objetos aos quais um synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="e1302-116">The identifiers of one or more objects to which a synchronizationJob is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1302-117">Relações</span><span class="sxs-lookup"><span data-stu-id="e1302-117">Relationships</span></span>
<span data-ttu-id="e1302-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e1302-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1302-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e1302-119">JSON representation</span></span>
<span data-ttu-id="e1302-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e1302-120">The following is a JSON representation of the resource.</span></span>
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
