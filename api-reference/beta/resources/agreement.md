---
title: tipo de recurso de contrato
description: Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o recurso termos de uso do Azure Active Directory de acordo com seu cenário.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9d45be38338554a1bf5181e4f7a3624b3d928127
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508384"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="e11bc-104">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="e11bc-104">agreement resource type</span></span>

<span data-ttu-id="e11bc-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e11bc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e11bc-106">Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e11bc-106">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="e11bc-107">Você pode usar os métodos a seguir para criar e gerenciar o [recurso termos de uso do Azure Active Directory de](/azure/active-directory/active-directory-tou) acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="e11bc-107">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="e11bc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="e11bc-108">Methods</span></span>

| <span data-ttu-id="e11bc-109">Método</span><span class="sxs-lookup"><span data-stu-id="e11bc-109">Method</span></span>       | <span data-ttu-id="e11bc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e11bc-110">Return Type</span></span> | <span data-ttu-id="e11bc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e11bc-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="e11bc-112">Criar contratos</span><span class="sxs-lookup"><span data-stu-id="e11bc-112">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="e11bc-113">contrato</span><span class="sxs-lookup"><span data-stu-id="e11bc-113">agreement</span></span>](agreement.md) | <span data-ttu-id="e11bc-114">Crie um novo contrato postando na coleção de contratos.</span><span class="sxs-lookup"><span data-stu-id="e11bc-114">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="e11bc-115">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="e11bc-115">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="e11bc-116">coleção de [contratos](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="e11bc-116">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="e11bc-117">Obtenha uma coleção de objetos de contrato.</span><span class="sxs-lookup"><span data-stu-id="e11bc-117">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="e11bc-118">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="e11bc-118">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="e11bc-119">contrato</span><span class="sxs-lookup"><span data-stu-id="e11bc-119">agreement</span></span>](agreement.md) | <span data-ttu-id="e11bc-120">Leia as propriedades e as relações de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="e11bc-120">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="e11bc-121">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="e11bc-121">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="e11bc-122">contrato</span><span class="sxs-lookup"><span data-stu-id="e11bc-122">agreement</span></span>](agreement.md) | <span data-ttu-id="e11bc-123">Atualize um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="e11bc-123">Update an agreement object.</span></span> |
| [<span data-ttu-id="e11bc-124">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="e11bc-124">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="e11bc-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e11bc-125">None</span></span> | <span data-ttu-id="e11bc-126">Exclua um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="e11bc-126">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="e11bc-127">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e11bc-127">Properties</span></span>
| <span data-ttu-id="e11bc-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e11bc-128">Property</span></span>     | <span data-ttu-id="e11bc-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e11bc-129">Type</span></span>        | <span data-ttu-id="e11bc-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e11bc-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e11bc-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e11bc-131">displayName</span></span>|<span data-ttu-id="e11bc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e11bc-132">String</span></span>|<span data-ttu-id="e11bc-133">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="e11bc-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="e11bc-134">id</span><span class="sxs-lookup"><span data-stu-id="e11bc-134">id</span></span>|<span data-ttu-id="e11bc-135">String</span><span class="sxs-lookup"><span data-stu-id="e11bc-135">String</span></span>| <span data-ttu-id="e11bc-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e11bc-136">Read-only.</span></span>|
|<span data-ttu-id="e11bc-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="e11bc-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="e11bc-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11bc-138">Boolean</span></span>|<span data-ttu-id="e11bc-139">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="e11bc-139">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e11bc-140">Relações</span><span class="sxs-lookup"><span data-stu-id="e11bc-140">Relationships</span></span>
| <span data-ttu-id="e11bc-141">Relação</span><span class="sxs-lookup"><span data-stu-id="e11bc-141">Relationship</span></span> | <span data-ttu-id="e11bc-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="e11bc-142">Type</span></span>        | <span data-ttu-id="e11bc-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="e11bc-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e11bc-144">arquivos</span><span class="sxs-lookup"><span data-stu-id="e11bc-144">files</span></span>|<span data-ttu-id="e11bc-145">coleção [agreementfile](agreementfile.md)</span><span class="sxs-lookup"><span data-stu-id="e11bc-145">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="e11bc-146">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e11bc-146">Read-only.</span></span> <span data-ttu-id="e11bc-147">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="e11bc-147">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e11bc-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e11bc-148">JSON representation</span></span>

<span data-ttu-id="e11bc-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e11bc-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
