---
title: tipo de recurso webaccount
description: tipo de recurso webaccount
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 414e3f491736f51ee670390519241110bc81f66e
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2019
ms.locfileid: "37950352"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="de820-103">tipo de recurso webaccount</span><span class="sxs-lookup"><span data-stu-id="de820-103">webAccount resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de820-104">Representa contas da Web que o usuário indicou que usa ou adicionou ao [perfil](profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="de820-104">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="de820-105">Esse tipo de recurso herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="de820-105">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="de820-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="de820-106">Methods</span></span>

| <span data-ttu-id="de820-107">Método</span><span class="sxs-lookup"><span data-stu-id="de820-107">Method</span></span>                                     | <span data-ttu-id="de820-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="de820-108">Return Type</span></span>                 | <span data-ttu-id="de820-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="de820-109">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="de820-110">Obter webaccount</span><span class="sxs-lookup"><span data-stu-id="de820-110">Get webAccount</span></span>](../api/webaccount-get.md) | [<span data-ttu-id="de820-111">conta da</span><span class="sxs-lookup"><span data-stu-id="de820-111">webAccount</span></span>](webaccount.md) | <span data-ttu-id="de820-112">Leia as propriedades e os relacionamentos de um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="de820-112">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="de820-113">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="de820-113">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="de820-114">conta da</span><span class="sxs-lookup"><span data-stu-id="de820-114">webAccount</span></span>](webaccount.md) | <span data-ttu-id="de820-115">Atualize um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="de820-115">Update a **webAccount** object.</span></span>                               |
| [<span data-ttu-id="de820-116">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="de820-116">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="de820-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de820-117">None</span></span>                        | <span data-ttu-id="de820-118">Excluir um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="de820-118">Delete a **webAccount** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="de820-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de820-119">Properties</span></span>

| <span data-ttu-id="de820-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de820-120">Property</span></span>     | <span data-ttu-id="de820-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="de820-121">Type</span></span>                                      | <span data-ttu-id="de820-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="de820-122">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="de820-123">description</span><span class="sxs-lookup"><span data-stu-id="de820-123">description</span></span>   |<span data-ttu-id="de820-124">String</span><span class="sxs-lookup"><span data-stu-id="de820-124">String</span></span>                                     | <span data-ttu-id="de820-125">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="de820-125">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="de820-126">service</span><span class="sxs-lookup"><span data-stu-id="de820-126">service</span></span>       |[<span data-ttu-id="de820-127">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="de820-127">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="de820-128">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="de820-128">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="de820-129">statusMessage</span><span class="sxs-lookup"><span data-stu-id="de820-129">statusMessage</span></span> |<span data-ttu-id="de820-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de820-130">String</span></span>                                     | <span data-ttu-id="de820-131">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="de820-131">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="de820-132">userId</span><span class="sxs-lookup"><span data-stu-id="de820-132">userId</span></span>        |<span data-ttu-id="de820-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="de820-133">String</span></span>                                     | <span data-ttu-id="de820-134">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="de820-134">The user name  displayed for the webaccount.</span></span>                                    |
|<span data-ttu-id="de820-135">webUrl</span><span class="sxs-lookup"><span data-stu-id="de820-135">webUrl</span></span>        |<span data-ttu-id="de820-136">String</span><span class="sxs-lookup"><span data-stu-id="de820-136">String</span></span>                                     | <span data-ttu-id="de820-137">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="de820-137">Contains a link to the user's profile on the cloud service if one exists.</span></span>                       |

## <a name="relationships"></a><span data-ttu-id="de820-138">Relações</span><span class="sxs-lookup"><span data-stu-id="de820-138">Relationships</span></span>

<span data-ttu-id="de820-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de820-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de820-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de820-140">JSON representation</span></span>

<span data-ttu-id="de820-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de820-141">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.webAccount",
  "baseType": ""
}-->

```json
{
  "description": "String",
  "service": {"@odata.type": "microsoft.graph.serviceInformation"},
  "statusMessage": "String",
  "userId": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webAccount resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
