---
title: tipo de recurso PersonName
description: tipo de recurso PersonName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: aad97177a06933d2dd98c5cc94744450197f7dcb
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939597"
---
# <a name="personname-resource-type"></a><span data-ttu-id="19204-103">tipo de recurso PersonName</span><span class="sxs-lookup"><span data-stu-id="19204-103">personName resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19204-104">Representa as informações de nome estendidas fornecidas pelo usuário ou que elas associaram à conta.</span><span class="sxs-lookup"><span data-stu-id="19204-104">Represents extended name information provided by the user or which they have associated with their account.</span></span>

<span data-ttu-id="19204-105">Herda de [Myfacet](itemfacet.md).</span><span class="sxs-lookup"><span data-stu-id="19204-105">Inherits from [itemFacet](itemfacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="19204-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="19204-106">Methods</span></span>

| <span data-ttu-id="19204-107">Método</span><span class="sxs-lookup"><span data-stu-id="19204-107">Method</span></span>                                     | <span data-ttu-id="19204-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="19204-108">Return Type</span></span>                 | <span data-ttu-id="19204-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="19204-109">Description</span></span>                                             |
|:-------------------------------------------|:----------------------------|:--------------------------------------------------------|
| [<span data-ttu-id="19204-110">Obter PersonName</span><span class="sxs-lookup"><span data-stu-id="19204-110">Get personName</span></span>](../api/personname-get.md) | [<span data-ttu-id="19204-111">personName</span><span class="sxs-lookup"><span data-stu-id="19204-111">personName</span></span>](personname.md) | <span data-ttu-id="19204-112">Leia as propriedades e as relações do objeto PersonName.</span><span class="sxs-lookup"><span data-stu-id="19204-112">Read properties and relationships of personName object.</span></span> |
| [<span data-ttu-id="19204-113">Update</span><span class="sxs-lookup"><span data-stu-id="19204-113">Update</span></span>](../api/personname-update.md)      | [<span data-ttu-id="19204-114">personName</span><span class="sxs-lookup"><span data-stu-id="19204-114">personName</span></span>](personname.md) | <span data-ttu-id="19204-115">Objeto Update PersonName.</span><span class="sxs-lookup"><span data-stu-id="19204-115">Update personName object.</span></span>                               |
| [<span data-ttu-id="19204-116">Delete</span><span class="sxs-lookup"><span data-stu-id="19204-116">Delete</span></span>](../api/personname-delete.md)      | <span data-ttu-id="19204-117">None</span><span class="sxs-lookup"><span data-stu-id="19204-117">None</span></span>                        | <span data-ttu-id="19204-118">Exclua o objeto PersonName.</span><span class="sxs-lookup"><span data-stu-id="19204-118">Delete personName object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="19204-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19204-119">Properties</span></span>

| <span data-ttu-id="19204-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19204-120">Property</span></span>     | <span data-ttu-id="19204-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="19204-121">Type</span></span>                              | <span data-ttu-id="19204-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="19204-122">Description</span></span> |
|:-------------|:----------------------------------|:------------|
|<span data-ttu-id="19204-123">displayName</span><span class="sxs-lookup"><span data-stu-id="19204-123">displayName</span></span>   |<span data-ttu-id="19204-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="19204-124">String</span></span>                             | <span data-ttu-id="19204-125">Fornece uma renderização ordenada de firstName e lastName, dependendo da localidade do usuário ou de seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="19204-125">Provides an ordered rendering of firstName and lastName depending on the locale of the user or their device.</span></span> |
|<span data-ttu-id="19204-126">primeiro</span><span class="sxs-lookup"><span data-stu-id="19204-126">first</span></span>         |<span data-ttu-id="19204-127">String</span><span class="sxs-lookup"><span data-stu-id="19204-127">String</span></span>                             | <span data-ttu-id="19204-128">Nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="19204-128">First Name of the user.</span></span>                                                                                      |
|<span data-ttu-id="19204-129">initials</span><span class="sxs-lookup"><span data-stu-id="19204-129">initials</span></span>      |<span data-ttu-id="19204-130">String</span><span class="sxs-lookup"><span data-stu-id="19204-130">String</span></span>                             | <span data-ttu-id="19204-131">Iniciais do usuário.</span><span class="sxs-lookup"><span data-stu-id="19204-131">Initials of the user.</span></span>                                                                                        |
|<span data-ttu-id="19204-132">languageTag</span><span class="sxs-lookup"><span data-stu-id="19204-132">languageTag</span></span>   |<span data-ttu-id="19204-133">String</span><span class="sxs-lookup"><span data-stu-id="19204-133">String</span></span>                             | <span data-ttu-id="19204-134">Contém o nome do idioma (en-US, no-NB, en-AU) após o formato BCP47 da IETF.</span><span class="sxs-lookup"><span data-stu-id="19204-134">Contains the name for the language (en-US, no-NB, en-AU) following IETF BCP47 format.</span></span>                        |
|<span data-ttu-id="19204-135">durar</span><span class="sxs-lookup"><span data-stu-id="19204-135">last</span></span>          |<span data-ttu-id="19204-136">String</span><span class="sxs-lookup"><span data-stu-id="19204-136">String</span></span>                             | <span data-ttu-id="19204-137">Sobrenome do usuário.</span><span class="sxs-lookup"><span data-stu-id="19204-137">Last Name of the user.</span></span>                                                                                       |
|<span data-ttu-id="19204-138">Virgem</span><span class="sxs-lookup"><span data-stu-id="19204-138">maiden</span></span>        |<span data-ttu-id="19204-139">String</span><span class="sxs-lookup"><span data-stu-id="19204-139">String</span></span>                             | <span data-ttu-id="19204-140">Nome de solteira do usuário.</span><span class="sxs-lookup"><span data-stu-id="19204-140">Maiden Name of the user.</span></span>                                                                                     |
|<span data-ttu-id="19204-141">middleware</span><span class="sxs-lookup"><span data-stu-id="19204-141">middle</span></span>        |<span data-ttu-id="19204-142">String</span><span class="sxs-lookup"><span data-stu-id="19204-142">String</span></span>                             | <span data-ttu-id="19204-143">Middlie nome do usuário.</span><span class="sxs-lookup"><span data-stu-id="19204-143">Middlie Name of the user.</span></span>                                                                                    | 
|<span data-ttu-id="19204-144">apelido</span><span class="sxs-lookup"><span data-stu-id="19204-144">nickname</span></span>      |<span data-ttu-id="19204-145">String</span><span class="sxs-lookup"><span data-stu-id="19204-145">String</span></span>                             | <span data-ttu-id="19204-146">Apelido do usuário.</span><span class="sxs-lookup"><span data-stu-id="19204-146">Nickname of the user.</span></span>                                                                                        |
|<span data-ttu-id="19204-147">pronúncia</span><span class="sxs-lookup"><span data-stu-id="19204-147">pronunciation</span></span> |[<span data-ttu-id="19204-148">yomiPersonName</span><span class="sxs-lookup"><span data-stu-id="19204-148">yomiPersonName</span></span>](yomipersonname.md)| <span data-ttu-id="19204-149">Orientações sobre como pronunciar o nome dos usuários.</span><span class="sxs-lookup"><span data-stu-id="19204-149">Guidance on how to pronounce the users name.</span></span>                                                                 |
|<span data-ttu-id="19204-150">sufixo</span><span class="sxs-lookup"><span data-stu-id="19204-150">suffix</span></span>        |<span data-ttu-id="19204-151">String</span><span class="sxs-lookup"><span data-stu-id="19204-151">String</span></span>                             | <span data-ttu-id="19204-152">Designadores usados após o nome dos usuários (por exemplo: PhD).</span><span class="sxs-lookup"><span data-stu-id="19204-152">Designators used after the users name (eg: PhD.)</span></span>                                                             |
|<span data-ttu-id="19204-153">title</span><span class="sxs-lookup"><span data-stu-id="19204-153">title</span></span>         |<span data-ttu-id="19204-154">String</span><span class="sxs-lookup"><span data-stu-id="19204-154">String</span></span>                             | <span data-ttu-id="19204-155">Honorifics usado para prefixar um nome de usuário (por exemplo: Dr, Sir, Madam, Sra.)</span><span class="sxs-lookup"><span data-stu-id="19204-155">Honorifics used to prefix a users name (eg: Dr, Sir, Madam, Mrs.)</span></span>                                            |

## <a name="relationships"></a><span data-ttu-id="19204-156">Relações</span><span class="sxs-lookup"><span data-stu-id="19204-156">Relationships</span></span>

<span data-ttu-id="19204-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="19204-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19204-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19204-158">JSON representation</span></span>

<span data-ttu-id="19204-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="19204-159">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personName",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "first": "String",
  "initials": "String",
  "languageTag": "String",
  "last": "String",
  "maiden": "String",
  "middle": "String",
  "nickname": "String",
  "pronunciation": {"@odata.type": "microsoft.graph.yomiPersonName"},
  "suffix": "String",
  "title": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personName resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->