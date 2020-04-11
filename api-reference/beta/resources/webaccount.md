---
title: tipo de recurso webaccount
description: tipo de recurso webaccount
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: dbdae8f0035e92b1c5b74c0ef3f842d2eb5af37a
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43228863"
---
# <a name="webaccount-resource-type"></a><span data-ttu-id="b61bf-103">tipo de recurso webaccount</span><span class="sxs-lookup"><span data-stu-id="b61bf-103">webAccount resource type</span></span>

<span data-ttu-id="b61bf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b61bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b61bf-105">Representa contas da Web que o usuário indicou que usa ou adicionou ao [perfil](profile.md)do usuário.</span><span class="sxs-lookup"><span data-stu-id="b61bf-105">Represents web accounts the user has indicated they use or has added to their user [profile](profile.md).</span></span>

<span data-ttu-id="b61bf-106">Esse tipo de recurso herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="b61bf-106">This resource type inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b61bf-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b61bf-107">Methods</span></span>

| <span data-ttu-id="b61bf-108">Método</span><span class="sxs-lookup"><span data-stu-id="b61bf-108">Method</span></span>                                                | <span data-ttu-id="b61bf-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b61bf-109">Return Type</span></span>                 | <span data-ttu-id="b61bf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b61bf-110">Description</span></span>                                                       |
|:------------------------------------------------------|:----------------------------|:------------------------------------------------------------------|
| [<span data-ttu-id="b61bf-111">Obter webaccount</span><span class="sxs-lookup"><span data-stu-id="b61bf-111">Get webAccount</span></span>](../api/webaccount-get.md)            | [<span data-ttu-id="b61bf-112">conta da</span><span class="sxs-lookup"><span data-stu-id="b61bf-112">webAccount</span></span>](webaccount.md) | <span data-ttu-id="b61bf-113">Leia as propriedades e os relacionamentos de um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="b61bf-113">Read the properties and relationships of a **webAccount** object.</span></span> |
| [<span data-ttu-id="b61bf-114">Atualizar webaccount</span><span class="sxs-lookup"><span data-stu-id="b61bf-114">Update webAccount</span></span>](../api/webaccount-update.md)      | [<span data-ttu-id="b61bf-115">conta da</span><span class="sxs-lookup"><span data-stu-id="b61bf-115">webAccount</span></span>](webaccount.md) | <span data-ttu-id="b61bf-116">Atualize um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="b61bf-116">Update a **webAccount** object.</span></span>                                   |
| [<span data-ttu-id="b61bf-117">Excluir conta da</span><span class="sxs-lookup"><span data-stu-id="b61bf-117">Delete webAccount</span></span>](../api/webaccount-delete.md)      | <span data-ttu-id="b61bf-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b61bf-118">None</span></span>                        | <span data-ttu-id="b61bf-119">Excluir um objeto **webaccount** .</span><span class="sxs-lookup"><span data-stu-id="b61bf-119">Delete a **webAccount** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="b61bf-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b61bf-120">Properties</span></span>

| <span data-ttu-id="b61bf-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b61bf-121">Property</span></span>     | <span data-ttu-id="b61bf-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b61bf-122">Type</span></span>                                      | <span data-ttu-id="b61bf-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b61bf-123">Description</span></span>                                                                                    |
|:-------------|:------------------------------------------|:-----------------------------------------------------------------------------------------------|
|<span data-ttu-id="b61bf-124">description</span><span class="sxs-lookup"><span data-stu-id="b61bf-124">description</span></span>   |<span data-ttu-id="b61bf-125">String</span><span class="sxs-lookup"><span data-stu-id="b61bf-125">String</span></span>                                     | <span data-ttu-id="b61bf-126">Contém a descrição que o usuário forneceu para a conta no serviço que está sendo referenciado.</span><span class="sxs-lookup"><span data-stu-id="b61bf-126">Contains the description the user has provided for the account on the service being referenced.</span></span>|
|<span data-ttu-id="b61bf-127">service</span><span class="sxs-lookup"><span data-stu-id="b61bf-127">service</span></span>       |[<span data-ttu-id="b61bf-128">Informações sobre o</span><span class="sxs-lookup"><span data-stu-id="b61bf-128">serviceInformation</span></span>](serviceinformation.md)| <span data-ttu-id="b61bf-129">Contém detalhes básicos sobre o serviço que está sendo associado.</span><span class="sxs-lookup"><span data-stu-id="b61bf-129">Contains basic detail about the service that is being associated.</span></span>                              |
|<span data-ttu-id="b61bf-130">statusMessage</span><span class="sxs-lookup"><span data-stu-id="b61bf-130">statusMessage</span></span> |<span data-ttu-id="b61bf-131">String</span><span class="sxs-lookup"><span data-stu-id="b61bf-131">String</span></span>                                     | <span data-ttu-id="b61bf-132">Contém uma mensagem de status do serviço de nuvem, se fornecido ou sincronizado.</span><span class="sxs-lookup"><span data-stu-id="b61bf-132">Contains a status message from the cloud service if provided or synchronized.</span></span>                  |
|<span data-ttu-id="b61bf-133">userId</span><span class="sxs-lookup"><span data-stu-id="b61bf-133">userId</span></span>        |<span data-ttu-id="b61bf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b61bf-134">String</span></span>                                     | <span data-ttu-id="b61bf-135">O nome de usuário exibido para a conta da Web.</span><span class="sxs-lookup"><span data-stu-id="b61bf-135">The user name  displayed for the webaccount.</span></span>                                                   |
|<span data-ttu-id="b61bf-136">webUrl</span><span class="sxs-lookup"><span data-stu-id="b61bf-136">webUrl</span></span>        |<span data-ttu-id="b61bf-137">String</span><span class="sxs-lookup"><span data-stu-id="b61bf-137">String</span></span>                                     | <span data-ttu-id="b61bf-138">Contém um link para o perfil do usuário no serviço de nuvem, se houver um.</span><span class="sxs-lookup"><span data-stu-id="b61bf-138">Contains a link to the user's profile on the cloud service if one exists.</span></span>                      |

## <a name="relationships"></a><span data-ttu-id="b61bf-139">Relações</span><span class="sxs-lookup"><span data-stu-id="b61bf-139">Relationships</span></span>

<span data-ttu-id="b61bf-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b61bf-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b61bf-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b61bf-141">JSON representation</span></span>

<span data-ttu-id="b61bf-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b61bf-142">The following is a JSON representation of the resource.</span></span>

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
