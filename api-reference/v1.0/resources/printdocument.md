---
title: Tipo de recurso printDocument
description: Representa um documento que está sendo impresso.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: d8ca73a6e8acfb6ac2326b171b2b8c04fed7e039
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516913"
---
# <a name="printdocument-resource-type"></a><span data-ttu-id="2742c-103">Tipo de recurso printDocument</span><span class="sxs-lookup"><span data-stu-id="2742c-103">printDocument resource type</span></span>

<span data-ttu-id="2742c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2742c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2742c-105">Representa um documento que está sendo impresso.</span><span class="sxs-lookup"><span data-stu-id="2742c-105">Represents a document being printed.</span></span>

## <a name="methods"></a><span data-ttu-id="2742c-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="2742c-106">Methods</span></span>
|<span data-ttu-id="2742c-107">Método</span><span class="sxs-lookup"><span data-stu-id="2742c-107">Method</span></span>|<span data-ttu-id="2742c-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2742c-108">Return type</span></span>|<span data-ttu-id="2742c-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2742c-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="2742c-110">Criar sessão de carregamento</span><span class="sxs-lookup"><span data-stu-id="2742c-110">Create upload session</span></span>](../api/printdocument-createuploadsession.md) | [<span data-ttu-id="2742c-111">uploadSession</span><span class="sxs-lookup"><span data-stu-id="2742c-111">uploadSession</span></span>](uploadsession.md) | <span data-ttu-id="2742c-112">Criar uma sessão de carregamento para carregar iterativamente intervalos de arquivo binário do **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="2742c-112">Create an upload session to iteratively upload ranges of binary file of the **printDocument**.</span></span> |
| [<span data-ttu-id="2742c-113">Baixar arquivo binário</span><span class="sxs-lookup"><span data-stu-id="2742c-113">Download binary file</span></span>](../api/printdocument-get-file.md) | <span data-ttu-id="2742c-114">Baixar Url</span><span class="sxs-lookup"><span data-stu-id="2742c-114">Download Url</span></span> | <span data-ttu-id="2742c-115">Baixe o arquivo binário associado ao **printDocument**.</span><span class="sxs-lookup"><span data-stu-id="2742c-115">Download the binary file associated with the **printDocument**.</span></span> |

## <a name="properties"></a><span data-ttu-id="2742c-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2742c-116">Properties</span></span>
|<span data-ttu-id="2742c-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2742c-117">Property</span></span>|<span data-ttu-id="2742c-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="2742c-118">Type</span></span>|<span data-ttu-id="2742c-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="2742c-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2742c-120">id</span><span class="sxs-lookup"><span data-stu-id="2742c-120">id</span></span>|<span data-ttu-id="2742c-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2742c-121">String</span></span>|<span data-ttu-id="2742c-122">O identificador do documento.</span><span class="sxs-lookup"><span data-stu-id="2742c-122">The document's identifier.</span></span> <span data-ttu-id="2742c-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2742c-123">Read-only.</span></span>|
|<span data-ttu-id="2742c-124">displayName</span><span class="sxs-lookup"><span data-stu-id="2742c-124">displayName</span></span>|<span data-ttu-id="2742c-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2742c-125">String</span></span>|<span data-ttu-id="2742c-126">O nome do documento.</span><span class="sxs-lookup"><span data-stu-id="2742c-126">The document's name.</span></span> <span data-ttu-id="2742c-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2742c-127">Read-only.</span></span>|
|<span data-ttu-id="2742c-128">contentType</span><span class="sxs-lookup"><span data-stu-id="2742c-128">contentType</span></span>|<span data-ttu-id="2742c-129">String</span><span class="sxs-lookup"><span data-stu-id="2742c-129">String</span></span>|<span data-ttu-id="2742c-130">Tipo de conteúdo do documento (MIME).</span><span class="sxs-lookup"><span data-stu-id="2742c-130">The document's content (MIME) type.</span></span> <span data-ttu-id="2742c-131">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2742c-131">Read-only.</span></span>|
|<span data-ttu-id="2742c-132">size</span><span class="sxs-lookup"><span data-stu-id="2742c-132">size</span></span>|<span data-ttu-id="2742c-133">Int64</span><span class="sxs-lookup"><span data-stu-id="2742c-133">Int64</span></span>|<span data-ttu-id="2742c-134">O tamanho do documento em bytes.</span><span class="sxs-lookup"><span data-stu-id="2742c-134">The document's size in bytes.</span></span> <span data-ttu-id="2742c-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2742c-135">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2742c-136">Relações</span><span class="sxs-lookup"><span data-stu-id="2742c-136">Relationships</span></span>
<span data-ttu-id="2742c-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2742c-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2742c-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2742c-138">JSON representation</span></span>
<span data-ttu-id="2742c-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2742c-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printDocument",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printDocument",
  "id": "String (identifier)",
  "displayName": "String",
  "contentType": "String",
  "size": "Integer"
}
```