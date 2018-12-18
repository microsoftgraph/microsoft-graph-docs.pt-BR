---
title: Tipo de recurso WorksheetProtection
description: Representa a proteção de um objeto de planilha.
author: lumine2008
ms.openlocfilehash: 91415b067fbe54333e32d1a2ed84bce5025b7d3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339204"
---
# <a name="worksheetprotection-resource-type"></a><span data-ttu-id="4bca8-103">Tipo de recurso WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4bca8-103">WorksheetProtection resource type</span></span>

> <span data-ttu-id="4bca8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4bca8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4bca8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4bca8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4bca8-106">Representa a proteção de um objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="4bca8-106">Represents the protection of a sheet object.</span></span>


## <a name="methods"></a><span data-ttu-id="4bca8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4bca8-107">Methods</span></span>

| <span data-ttu-id="4bca8-108">Método</span><span class="sxs-lookup"><span data-stu-id="4bca8-108">Method</span></span>           | <span data-ttu-id="4bca8-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="4bca8-109">Return Type</span></span>    |<span data-ttu-id="4bca8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bca8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4bca8-111">Get WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4bca8-111">Get WorksheetProtection</span></span>](../api/worksheetprotection-get.md) | [<span data-ttu-id="4bca8-112">WorksheetProtection</span><span class="sxs-lookup"><span data-stu-id="4bca8-112">WorksheetProtection</span></span>](worksheetprotection.md) |<span data-ttu-id="4bca8-113">Leia as propriedades e os relacionamentos do objeto worksheetProtection.</span><span class="sxs-lookup"><span data-stu-id="4bca8-113">Read properties and relationships of worksheetProtection object.</span></span>|
|[<span data-ttu-id="4bca8-114">Protect</span><span class="sxs-lookup"><span data-stu-id="4bca8-114">Protect</span></span>](../api/worksheetprotection-protect.md)|<span data-ttu-id="4bca8-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4bca8-115">None</span></span>|<span data-ttu-id="4bca8-p102">Protege uma planilha. Gera uma exceção se a planilha estiver protegida.</span><span class="sxs-lookup"><span data-stu-id="4bca8-p102">Protect a worksheet. It throws if the worksheet has been protected.</span></span>|
|[<span data-ttu-id="4bca8-118">Unprotect</span><span class="sxs-lookup"><span data-stu-id="4bca8-118">Unprotect</span></span>](../api/worksheetprotection-unprotect.md)|<span data-ttu-id="4bca8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4bca8-119">None</span></span>|<span data-ttu-id="4bca8-120">Desprotege uma planilha.</span><span class="sxs-lookup"><span data-stu-id="4bca8-120">Unprotect a worksheet</span></span>|

## <a name="properties"></a><span data-ttu-id="4bca8-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4bca8-121">Properties</span></span>
| <span data-ttu-id="4bca8-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4bca8-122">Property</span></span>     | <span data-ttu-id="4bca8-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bca8-123">Type</span></span>   |<span data-ttu-id="4bca8-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bca8-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bca8-125">protected</span><span class="sxs-lookup"><span data-stu-id="4bca8-125">protected</span></span>|<span data-ttu-id="4bca8-126">booliano</span><span class="sxs-lookup"><span data-stu-id="4bca8-126">boolean</span></span>|<span data-ttu-id="4bca8-p103">Indica se a planilha está protegida.  Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4bca8-p103">Indicates if the worksheet is protected.  Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4bca8-129">Relações</span><span class="sxs-lookup"><span data-stu-id="4bca8-129">Relationships</span></span>
| <span data-ttu-id="4bca8-130">Relação</span><span class="sxs-lookup"><span data-stu-id="4bca8-130">Relationship</span></span> | <span data-ttu-id="4bca8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4bca8-131">Type</span></span>   |<span data-ttu-id="4bca8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4bca8-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4bca8-133">options</span><span class="sxs-lookup"><span data-stu-id="4bca8-133">options</span></span>|[<span data-ttu-id="4bca8-134">WorksheetProtectionOptions</span><span class="sxs-lookup"><span data-stu-id="4bca8-134">WorksheetProtectionOptions</span></span>](worksheetprotectionoptions.md)|<span data-ttu-id="4bca8-p104">Opções de proteção da planilha. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="4bca8-p104">Sheet protection options. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4bca8-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4bca8-137">JSON representation</span></span>

<span data-ttu-id="4bca8-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4bca8-138">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.worksheetProtection"
}-->

```json
{
  "protected": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetProtection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->