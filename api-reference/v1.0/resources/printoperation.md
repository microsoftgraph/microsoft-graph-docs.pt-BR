---
title: Tipo de recurso printOperation
description: Representa uma operação de impressão universal de longa duração. Classe base para tipos de operação como printerCreateOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 9a397a0166ad62a503027499e9e0f5fd4f127b1e
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517034"
---
# <a name="printoperation-resource-type"></a><span data-ttu-id="80e20-104">Tipo de recurso printOperation</span><span class="sxs-lookup"><span data-stu-id="80e20-104">printOperation resource type</span></span>

<span data-ttu-id="80e20-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80e20-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="80e20-106">Representa uma operação de impressão universal de longa duração.</span><span class="sxs-lookup"><span data-stu-id="80e20-106">Represents a long-running Universal Print operation.</span></span> <span data-ttu-id="80e20-107">Classe base para tipos de operação como [printerCreateOperation](printercreateoperation.md).</span><span class="sxs-lookup"><span data-stu-id="80e20-107">Base class for operation types such as [printerCreateOperation](printercreateoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="80e20-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="80e20-108">Methods</span></span>
|<span data-ttu-id="80e20-109">Método</span><span class="sxs-lookup"><span data-stu-id="80e20-109">Method</span></span>|<span data-ttu-id="80e20-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="80e20-110">Return type</span></span>|<span data-ttu-id="80e20-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="80e20-111">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="80e20-112">Obter operação</span><span class="sxs-lookup"><span data-stu-id="80e20-112">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="80e20-113">printOperation</span><span class="sxs-lookup"><span data-stu-id="80e20-113">printOperation</span></span>](printoperation.md) | <span data-ttu-id="80e20-114">Recupere uma operação de longa duração dentro do usuário atual ou do locatário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="80e20-114">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="80e20-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80e20-115">Properties</span></span>
|<span data-ttu-id="80e20-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80e20-116">Property</span></span>|<span data-ttu-id="80e20-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="80e20-117">Type</span></span>|<span data-ttu-id="80e20-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="80e20-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80e20-119">id</span><span class="sxs-lookup"><span data-stu-id="80e20-119">id</span></span>|<span data-ttu-id="80e20-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80e20-120">String</span></span>|<span data-ttu-id="80e20-121">O identificador da operação.</span><span class="sxs-lookup"><span data-stu-id="80e20-121">The operation's identifier.</span></span> <span data-ttu-id="80e20-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80e20-122">Read-only.</span></span>|
|<span data-ttu-id="80e20-123">status</span><span class="sxs-lookup"><span data-stu-id="80e20-123">status</span></span>|[<span data-ttu-id="80e20-124">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="80e20-124">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="80e20-125">O status da operação.</span><span class="sxs-lookup"><span data-stu-id="80e20-125">The status of the operation.</span></span> <span data-ttu-id="80e20-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80e20-126">Read-only.</span></span>|
|<span data-ttu-id="80e20-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80e20-127">createdDateTime</span></span>|<span data-ttu-id="80e20-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80e20-128">DateTimeOffset</span></span>|<span data-ttu-id="80e20-129">DateTimeOffset quando a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="80e20-129">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="80e20-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="80e20-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="80e20-131">Relações</span><span class="sxs-lookup"><span data-stu-id="80e20-131">Relationships</span></span>
<span data-ttu-id="80e20-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="80e20-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="80e20-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80e20-133">JSON representation</span></span>
<span data-ttu-id="80e20-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80e20-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)"
}
```

