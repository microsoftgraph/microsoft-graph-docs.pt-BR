---
title: tipo de recurso synchronizationJobSubject
description: Representa os objetos que serão provisionados durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 54f8271d3b11cce55cc3e7042ffcba84a330d798
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: Auto
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "45007137"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="ec04c-103">tipo de recurso synchronizationJobSubject</span><span class="sxs-lookup"><span data-stu-id="ec04c-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="ec04c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec04c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ec04c-105">Representa os objetos que serão provisionados durante o provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="ec04c-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="ec04c-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ec04c-106">Properties</span></span>
|<span data-ttu-id="ec04c-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ec04c-107">Property</span></span>|<span data-ttu-id="ec04c-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ec04c-108">Type</span></span>|<span data-ttu-id="ec04c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ec04c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec04c-110">objectId</span><span class="sxs-lookup"><span data-stu-id="ec04c-110">objectId</span></span>|<span data-ttu-id="ec04c-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ec04c-111">String</span></span>|<span data-ttu-id="ec04c-112">O identificador de um objeto ao qual synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="ec04c-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="ec04c-113">objecttypename</span><span class="sxs-lookup"><span data-stu-id="ec04c-113">objectTypeName</span></span>|<span data-ttu-id="ec04c-114">String</span><span class="sxs-lookup"><span data-stu-id="ec04c-114">String</span></span>|<span data-ttu-id="ec04c-115">O tipo do objeto para o qual um synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="ec04c-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec04c-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ec04c-116">Relationships</span></span>
<span data-ttu-id="ec04c-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ec04c-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec04c-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ec04c-118">JSON representation</span></span>
<span data-ttu-id="ec04c-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ec04c-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationJobSubject"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationJobSubject",
  "objectId": "String",
  "objectTypeName": "String"
}
```
