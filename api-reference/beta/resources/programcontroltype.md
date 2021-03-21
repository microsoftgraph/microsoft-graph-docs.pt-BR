---
title: Tipo de recurso programControlType
description: 'No recurso de revisões de acesso do Azure AD, o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se trata.  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: markwahl-msft
ms.openlocfilehash: 58c9ee3ade6e3969de9653f54c5181a66f087ea5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960359"
---
# <a name="programcontroltype-resource-type"></a><span data-ttu-id="60c07-103">Tipo de recurso programControlType</span><span class="sxs-lookup"><span data-stu-id="60c07-103">programControlType resource type</span></span>

<span data-ttu-id="60c07-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60c07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60c07-105">No recurso de revisões de acesso do Azure [AD,](accessreviews-root.md) o tipo de controle de programa é usado ao associar um controle a um programa, para indicar o tipo de revisão de acesso para o qual o controle se trata.</span><span class="sxs-lookup"><span data-stu-id="60c07-105">In the Azure AD [access reviews](accessreviews-root.md) feature, the program control type is used when associating a control to a program, to indicate the type of access review the control is for.</span></span>  

<span data-ttu-id="60c07-106">Os objetos do tipo de controle do programa são gerados automaticamente quando o administrador global inscarda o locatário para usar o recurso de críticas de acesso.</span><span class="sxs-lookup"><span data-stu-id="60c07-106">The program control type objects are automatically generated when the global administrator onboards the tenant to use the access reviews feature.</span></span>  <span data-ttu-id="60c07-107">Nenhum tipo de controle de programa adicional pode ser criado.</span><span class="sxs-lookup"><span data-stu-id="60c07-107">No additional program control types can be created.</span></span>


## <a name="methods"></a><span data-ttu-id="60c07-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="60c07-108">Methods</span></span>

| <span data-ttu-id="60c07-109">Método</span><span class="sxs-lookup"><span data-stu-id="60c07-109">Method</span></span>           | <span data-ttu-id="60c07-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="60c07-110">Return Type</span></span>    |<span data-ttu-id="60c07-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c07-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60c07-112">Listar programControlTypes</span><span class="sxs-lookup"><span data-stu-id="60c07-112">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="60c07-113">[Coleção programControlType](programcontroltype.md)</span><span class="sxs-lookup"><span data-stu-id="60c07-113">[programControlType](programcontroltype.md) collection</span></span>| <span data-ttu-id="60c07-114">Listar tipos de controle de programa.</span><span class="sxs-lookup"><span data-stu-id="60c07-114">List program control types.</span></span> |

## <a name="properties"></a><span data-ttu-id="60c07-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="60c07-115">Properties</span></span>
| <span data-ttu-id="60c07-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="60c07-116">Property</span></span>     | <span data-ttu-id="60c07-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="60c07-117">Type</span></span>   |<span data-ttu-id="60c07-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c07-118">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="60c07-119">id</span><span class="sxs-lookup"><span data-stu-id="60c07-119">id</span></span>                     |<span data-ttu-id="60c07-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60c07-120">String</span></span>                | <span data-ttu-id="60c07-121">O identificador atribuído ao recurso do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="60c07-121">The feature-assigned identifier of the program control type</span></span>                                      |
| <span data-ttu-id="60c07-122">displayName</span><span class="sxs-lookup"><span data-stu-id="60c07-122">displayName</span></span>            |<span data-ttu-id="60c07-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="60c07-123">String</span></span>                | <span data-ttu-id="60c07-124">O nome do tipo de controle do programa</span><span class="sxs-lookup"><span data-stu-id="60c07-124">The name of the program control type</span></span>                                                             |


## <a name="relationships"></a><span data-ttu-id="60c07-125">Relações</span><span class="sxs-lookup"><span data-stu-id="60c07-125">Relationships</span></span>

<span data-ttu-id="60c07-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="60c07-126">None.</span></span>


## <a name="see-also"></a><span data-ttu-id="60c07-127">Ver também</span><span class="sxs-lookup"><span data-stu-id="60c07-127">See also</span></span>

| <span data-ttu-id="60c07-128">Método</span><span class="sxs-lookup"><span data-stu-id="60c07-128">Method</span></span>           | <span data-ttu-id="60c07-129">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="60c07-129">Return Type</span></span>    |<span data-ttu-id="60c07-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="60c07-130">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="60c07-131">Criar programControl</span><span class="sxs-lookup"><span data-stu-id="60c07-131">Create programControl</span></span>](../api/programcontrol-create.md) |     [<span data-ttu-id="60c07-132">programControl</span><span class="sxs-lookup"><span data-stu-id="60c07-132">programControl</span></span>](programcontrol.md) |   <span data-ttu-id="60c07-133">Adicione um programControl a um programa.</span><span class="sxs-lookup"><span data-stu-id="60c07-133">Add a programControl to a program.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="60c07-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="60c07-134">JSON representation</span></span>

<span data-ttu-id="60c07-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="60c07-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.programControlType"
}-->

```json
{
 "id": "string (identifier)",
 "displayName": "string"
}

```

<!--
{
  "type": "#page.annotation",
  "description": "programControlType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


