---
title: Tipo de recurso synchronizationJobSubject
description: Representa os objetos que serão provisionados durante o provisionamento sob demanda.
author: ArvindHarinder1
localization_priority: Normal
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c9e6d83ed7024556954740e89edcc18f7b56ba04
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50131995"
---
# <a name="synchronizationjobsubject-resource-type"></a><span data-ttu-id="6ecb8-103">Tipo de recurso synchronizationJobSubject</span><span class="sxs-lookup"><span data-stu-id="6ecb8-103">synchronizationJobSubject resource type</span></span>

<span data-ttu-id="6ecb8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ecb8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6ecb8-105">Representa os objetos que serão provisionados durante o provisionamento sob demanda.</span><span class="sxs-lookup"><span data-stu-id="6ecb8-105">Represents the objects that will be provisioned during on-demand provisioning.</span></span>

## <a name="properties"></a><span data-ttu-id="6ecb8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ecb8-106">Properties</span></span>
|<span data-ttu-id="6ecb8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ecb8-107">Property</span></span>|<span data-ttu-id="6ecb8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ecb8-108">Type</span></span>|<span data-ttu-id="6ecb8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ecb8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ecb8-110">objectId</span><span class="sxs-lookup"><span data-stu-id="6ecb8-110">objectId</span></span>|<span data-ttu-id="6ecb8-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ecb8-111">String</span></span>|<span data-ttu-id="6ecb8-112">O identificador de um objeto ao qual um synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="6ecb8-112">The identifier of an object to which a synchronizationJob  is to be applied.</span></span>|
|<span data-ttu-id="6ecb8-113">objectTypeName</span><span class="sxs-lookup"><span data-stu-id="6ecb8-113">objectTypeName</span></span>|<span data-ttu-id="6ecb8-114">String</span><span class="sxs-lookup"><span data-stu-id="6ecb8-114">String</span></span>|<span data-ttu-id="6ecb8-115">O tipo do objeto ao qual um synchronizationJob deve ser aplicado.</span><span class="sxs-lookup"><span data-stu-id="6ecb8-115">The type of the object to which a synchronizationJob  is to be applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ecb8-116">Relações</span><span class="sxs-lookup"><span data-stu-id="6ecb8-116">Relationships</span></span>
<span data-ttu-id="6ecb8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ecb8-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ecb8-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ecb8-118">JSON representation</span></span>
<span data-ttu-id="6ecb8-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ecb8-119">The following is a JSON representation of the resource.</span></span>
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


