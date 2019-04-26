---
title: tipo de recurso de contrato
description: Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD). Você pode usar os métodos a seguir para criar e gerenciar o recurso termos de uso do Azure Active Directory de acordo com seu cenário.
localization_priority: Normal
ms.openlocfilehash: d91cc8f8180ffb706639fb42a8c68d711991602c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339171"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="ee104-104">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="ee104-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee104-105">Representa o contrato de termos de uso personalizável de um locatário que é criado e gerenciado com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ee104-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="ee104-106">Você pode usar os métodos a seguir para criar e gerenciar o [recurso termos de uso do Azure Active Directory de](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="ee104-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="ee104-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ee104-107">Methods</span></span>

| <span data-ttu-id="ee104-108">Método</span><span class="sxs-lookup"><span data-stu-id="ee104-108">Method</span></span>       | <span data-ttu-id="ee104-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ee104-109">Return Type</span></span> | <span data-ttu-id="ee104-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee104-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="ee104-111">Criar contratos</span><span class="sxs-lookup"><span data-stu-id="ee104-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="ee104-112">contrato</span><span class="sxs-lookup"><span data-stu-id="ee104-112">agreement</span></span>](agreement.md) | <span data-ttu-id="ee104-113">Crie um novo contrato postando na coleção de contratos.</span><span class="sxs-lookup"><span data-stu-id="ee104-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="ee104-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="ee104-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="ee104-115">coleção de [contratos](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="ee104-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="ee104-116">Obtenha uma coleção de objetos de contrato.</span><span class="sxs-lookup"><span data-stu-id="ee104-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="ee104-117">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="ee104-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="ee104-118">contrato</span><span class="sxs-lookup"><span data-stu-id="ee104-118">agreement</span></span>](agreement.md) | <span data-ttu-id="ee104-119">Leia as propriedades e as relações de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="ee104-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="ee104-120">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="ee104-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="ee104-121">contrato</span><span class="sxs-lookup"><span data-stu-id="ee104-121">agreement</span></span>](agreement.md) | <span data-ttu-id="ee104-122">Atualize um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="ee104-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="ee104-123">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="ee104-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="ee104-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ee104-124">None</span></span> | <span data-ttu-id="ee104-125">Exclua um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="ee104-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="ee104-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ee104-126">Properties</span></span>
| <span data-ttu-id="ee104-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ee104-127">Property</span></span>     | <span data-ttu-id="ee104-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee104-128">Type</span></span>        | <span data-ttu-id="ee104-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee104-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee104-130">displayName</span><span class="sxs-lookup"><span data-stu-id="ee104-130">displayName</span></span>|<span data-ttu-id="ee104-131">String</span><span class="sxs-lookup"><span data-stu-id="ee104-131">String</span></span>|<span data-ttu-id="ee104-132">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="ee104-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="ee104-133">id</span><span class="sxs-lookup"><span data-stu-id="ee104-133">id</span></span>|<span data-ttu-id="ee104-134">String</span><span class="sxs-lookup"><span data-stu-id="ee104-134">String</span></span>| <span data-ttu-id="ee104-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee104-135">Read-only.</span></span>|
|<span data-ttu-id="ee104-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="ee104-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="ee104-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee104-137">Boolean</span></span>|<span data-ttu-id="ee104-138">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="ee104-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ee104-139">Relações</span><span class="sxs-lookup"><span data-stu-id="ee104-139">Relationships</span></span>
| <span data-ttu-id="ee104-140">Relação</span><span class="sxs-lookup"><span data-stu-id="ee104-140">Relationship</span></span> | <span data-ttu-id="ee104-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="ee104-141">Type</span></span>        | <span data-ttu-id="ee104-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="ee104-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ee104-143">arquivos</span><span class="sxs-lookup"><span data-stu-id="ee104-143">files</span></span>|<span data-ttu-id="ee104-144">[](agreementfile.md) coleção agreementfile</span><span class="sxs-lookup"><span data-stu-id="ee104-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="ee104-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ee104-145">Read-only.</span></span> <span data-ttu-id="ee104-146">PDFs vinculados a este contrato.</span><span class="sxs-lookup"><span data-stu-id="ee104-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ee104-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ee104-147">JSON representation</span></span>

<span data-ttu-id="ee104-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ee104-148">The following is a JSON representation of the resource.</span></span>

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
