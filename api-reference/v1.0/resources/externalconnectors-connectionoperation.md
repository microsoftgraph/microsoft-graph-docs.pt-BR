---
title: Tipo de recurso connectionOperation
description: Descreve o status de uma solicitação assíncrona para criar um Pesquisa da Microsoft de conexão.
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: f81300c0fd2f895daccb816c86cdd7151c803b2d
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467202"
---
# <a name="connectionoperation-resource-type"></a><span data-ttu-id="277ec-103">Tipo de recurso connectionOperation</span><span class="sxs-lookup"><span data-stu-id="277ec-103">connectionOperation resource type</span></span>

<span data-ttu-id="277ec-104">Namespace: microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="277ec-104">Namespace: microsoft.graph.externalConnectors</span></span>



<span data-ttu-id="277ec-105">Descreve o status de uma solicitação assíncrona para criar um Pesquisa da Microsoft [de conexão](externalconnectors-schema.md).</span><span class="sxs-lookup"><span data-stu-id="277ec-105">Describes status of an asynchronous request to create a Microsoft Search connection [schema](externalconnectors-schema.md).</span></span>

## <a name="methods"></a><span data-ttu-id="277ec-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="277ec-106">Methods</span></span>
|<span data-ttu-id="277ec-107">Método</span><span class="sxs-lookup"><span data-stu-id="277ec-107">Method</span></span>|<span data-ttu-id="277ec-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="277ec-108">Return type</span></span>|<span data-ttu-id="277ec-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="277ec-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="277ec-110">Obter connectionOperation</span><span class="sxs-lookup"><span data-stu-id="277ec-110">Get connectionOperation</span></span>](../api/externalconnectors-connectionoperation-get.md)|[<span data-ttu-id="277ec-111">connectionOperation</span><span class="sxs-lookup"><span data-stu-id="277ec-111">connectionOperation</span></span>](../resources/externalconnectors-connectionoperation.md)|<span data-ttu-id="277ec-112">Leia as propriedades e as relações de um [objeto connectionOperation.](../resources/externalconnectors-connectionoperation.md)</span><span class="sxs-lookup"><span data-stu-id="277ec-112">Read the properties and relationships of a [connectionOperation](../resources/externalconnectors-connectionoperation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="277ec-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="277ec-113">Properties</span></span>
|<span data-ttu-id="277ec-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="277ec-114">Property</span></span>|<span data-ttu-id="277ec-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="277ec-115">Type</span></span>|<span data-ttu-id="277ec-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="277ec-116">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="277ec-117">erro</span><span class="sxs-lookup"><span data-stu-id="277ec-117">error</span></span>|<span data-ttu-id="277ec-118">publicError</span><span class="sxs-lookup"><span data-stu-id="277ec-118">publicError</span></span>| <span data-ttu-id="277ec-119">Se `status` for , fornece mais informações sobre o erro que causou a `failed` falha.</span><span class="sxs-lookup"><span data-stu-id="277ec-119">If `status` is `failed`, provides more information about the error that caused the failure.</span></span>|
|<span data-ttu-id="277ec-120">id</span><span class="sxs-lookup"><span data-stu-id="277ec-120">id</span></span>|<span data-ttu-id="277ec-121">String</span><span class="sxs-lookup"><span data-stu-id="277ec-121">String</span></span>| <span data-ttu-id="277ec-122">Identificador exclusivo da connectionOperation.</span><span class="sxs-lookup"><span data-stu-id="277ec-122">Unique identifier for the connectionOperation.</span></span> <span data-ttu-id="277ec-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="277ec-123">Read-only.</span></span> |
|<span data-ttu-id="277ec-124">status</span><span class="sxs-lookup"><span data-stu-id="277ec-124">status</span></span>|<span data-ttu-id="277ec-125">microsoft.graph.externalConnectors.connectionOperationStatus</span><span class="sxs-lookup"><span data-stu-id="277ec-125">microsoft.graph.externalConnectors.connectionOperationStatus</span></span>| <span data-ttu-id="277ec-126">Indica o status da operação assíncrona.</span><span class="sxs-lookup"><span data-stu-id="277ec-126">Indicates the status of the asynchronous operation.</span></span> <span data-ttu-id="277ec-127">Os valores possíveis são: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="277ec-127">Possible values are: `unspecified`, `inprogress`, `completed`, `failed`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="277ec-128">Relações</span><span class="sxs-lookup"><span data-stu-id="277ec-128">Relationships</span></span>
<span data-ttu-id="277ec-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="277ec-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="277ec-130">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="277ec-130">JSON representation</span></span>
<span data-ttu-id="277ec-131">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="277ec-131">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.connectionOperation",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "status": "String"
}
```

