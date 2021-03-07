---
title: Tipo de recurso printerCreateOperation
description: Representa uma operação de registro de impressora de longa duração. Derivado de printOperation.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 31d872ba84df3fcdd4f246cbd32b3668d21e57d5
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516824"
---
# <a name="printercreateoperation-resource-type"></a><span data-ttu-id="25555-104">Tipo de recurso printerCreateOperation</span><span class="sxs-lookup"><span data-stu-id="25555-104">printerCreateOperation resource type</span></span>

<span data-ttu-id="25555-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25555-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="25555-106">Representa uma operação de registro de impressora de longa duração.</span><span class="sxs-lookup"><span data-stu-id="25555-106">Represents a long-running printer registration operation.</span></span> <span data-ttu-id="25555-107">Derivado de [printOperation](printoperation.md).</span><span class="sxs-lookup"><span data-stu-id="25555-107">Derived from [printOperation](printoperation.md).</span></span>

<span data-ttu-id="25555-108">Herda de [printOperation](printoperation.md).</span><span class="sxs-lookup"><span data-stu-id="25555-108">Inherits from [printOperation](printoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="25555-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="25555-109">Methods</span></span>
|<span data-ttu-id="25555-110">Método</span><span class="sxs-lookup"><span data-stu-id="25555-110">Method</span></span>|<span data-ttu-id="25555-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="25555-111">Return type</span></span>|<span data-ttu-id="25555-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="25555-112">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="25555-113">Obter operação</span><span class="sxs-lookup"><span data-stu-id="25555-113">Get operation</span></span>](../api/printoperation-get.md) | [<span data-ttu-id="25555-114">printOperation</span><span class="sxs-lookup"><span data-stu-id="25555-114">printOperation</span></span>](printoperation.md) | <span data-ttu-id="25555-115">Recupere uma operação de longa duração dentro do usuário atual ou do locatário do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="25555-115">Retrieve a long-running operation within current user or app's tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="25555-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="25555-116">Properties</span></span>
|<span data-ttu-id="25555-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="25555-117">Property</span></span>|<span data-ttu-id="25555-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="25555-118">Type</span></span>|<span data-ttu-id="25555-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="25555-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25555-120">id</span><span class="sxs-lookup"><span data-stu-id="25555-120">id</span></span>|<span data-ttu-id="25555-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25555-121">String</span></span>|<span data-ttu-id="25555-122">O identificador da operação.</span><span class="sxs-lookup"><span data-stu-id="25555-122">The operation's identifier.</span></span> <span data-ttu-id="25555-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25555-123">Read-only.</span></span>|
|<span data-ttu-id="25555-124">status</span><span class="sxs-lookup"><span data-stu-id="25555-124">status</span></span>|[<span data-ttu-id="25555-125">printOperationStatus</span><span class="sxs-lookup"><span data-stu-id="25555-125">printOperationStatus</span></span>](printoperationstatus.md)|<span data-ttu-id="25555-126">O status da operação de registro.</span><span class="sxs-lookup"><span data-stu-id="25555-126">The status of the registration operation.</span></span> <span data-ttu-id="25555-127">Contém o progresso da operação e se ela foi concluída com êxito.</span><span class="sxs-lookup"><span data-stu-id="25555-127">Contains the operation's progress and whether it completed successfully.</span></span> <span data-ttu-id="25555-128">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25555-128">Read-only.</span></span>|
|<span data-ttu-id="25555-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25555-129">createdDateTime</span></span>|<span data-ttu-id="25555-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25555-130">DateTimeOffset</span></span>|<span data-ttu-id="25555-131">DateTimeOffset quando a operação foi criada.</span><span class="sxs-lookup"><span data-stu-id="25555-131">The DateTimeOffset when the operation was created.</span></span> <span data-ttu-id="25555-132">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25555-132">Read-only.</span></span>|
|<span data-ttu-id="25555-133">certificado</span><span class="sxs-lookup"><span data-stu-id="25555-133">certificate</span></span>|<span data-ttu-id="25555-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="25555-134">String</span></span>|<span data-ttu-id="25555-135">O certificado assinado criado durante o processo de registro.</span><span class="sxs-lookup"><span data-stu-id="25555-135">The signed certificate created during the registration process.</span></span> <span data-ttu-id="25555-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25555-136">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="25555-137">Relações</span><span class="sxs-lookup"><span data-stu-id="25555-137">Relationships</span></span>
|<span data-ttu-id="25555-138">Relação</span><span class="sxs-lookup"><span data-stu-id="25555-138">Relationship</span></span>|<span data-ttu-id="25555-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="25555-139">Type</span></span>|<span data-ttu-id="25555-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="25555-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25555-141">impressora</span><span class="sxs-lookup"><span data-stu-id="25555-141">printer</span></span>|[<span data-ttu-id="25555-142">impressora</span><span class="sxs-lookup"><span data-stu-id="25555-142">printer</span></span>](printer.md)|<span data-ttu-id="25555-143">A entidade de impressora criada.</span><span class="sxs-lookup"><span data-stu-id="25555-143">The created printer entity.</span></span> <span data-ttu-id="25555-144">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="25555-144">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="25555-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="25555-145">JSON representation</span></span>
<span data-ttu-id="25555-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="25555-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printerCreateOperation",
  "baseType": "microsoft.graph.printOperation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerCreateOperation",
  "id": "String (identifier)",
  "status": {
    "@odata.type": "microsoft.graph.printOperationStatus"
  },
  "createdDateTime": "String (timestamp)",
  "certificate": "String"
}
```

