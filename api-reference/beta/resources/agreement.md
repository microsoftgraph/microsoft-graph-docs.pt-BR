---
title: tipo de recurso de contrato
description: Representa os termos personalizável de um locatário contrato de uso que é criado e gerenciado com o Azure Active Directory (AD Azure). Você pode usar os métodos a seguir para criar e gerenciar o recurso do Windows Azure Active Directory termos de uso de acordo com o seu cenário.
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513848"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="eb597-104">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="eb597-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb597-105">Representa os termos personalizável de um locatário contrato de uso que é criado e gerenciado com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="eb597-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="eb597-106">Você pode usar os métodos a seguir para criar e gerenciar o [Azure Active Directory termos de uso de recurso](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="eb597-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="eb597-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb597-107">Methods</span></span>

| <span data-ttu-id="eb597-108">Método</span><span class="sxs-lookup"><span data-stu-id="eb597-108">Method</span></span>       | <span data-ttu-id="eb597-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb597-109">Return Type</span></span> | <span data-ttu-id="eb597-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb597-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="eb597-111">Criar contratos</span><span class="sxs-lookup"><span data-stu-id="eb597-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="eb597-112">contrato</span><span class="sxs-lookup"><span data-stu-id="eb597-112">agreement</span></span>](agreement.md) | <span data-ttu-id="eb597-113">Crie um novo contrato pelo lançamento à coleção contrato.</span><span class="sxs-lookup"><span data-stu-id="eb597-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="eb597-114">Contratos de lista</span><span class="sxs-lookup"><span data-stu-id="eb597-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="eb597-115">coleção de [contrato](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="eb597-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="eb597-116">Obtenha uma coleção de objetos do contrato.</span><span class="sxs-lookup"><span data-stu-id="eb597-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="eb597-117">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="eb597-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="eb597-118">contrato</span><span class="sxs-lookup"><span data-stu-id="eb597-118">agreement</span></span>](agreement.md) | <span data-ttu-id="eb597-119">Leia as propriedades e os relacionamentos de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="eb597-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="eb597-120">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="eb597-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="eb597-121">contrato</span><span class="sxs-lookup"><span data-stu-id="eb597-121">agreement</span></span>](agreement.md) | <span data-ttu-id="eb597-122">Atualize um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="eb597-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="eb597-123">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="eb597-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="eb597-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb597-124">None</span></span> | <span data-ttu-id="eb597-125">Exclua um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="eb597-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="eb597-126">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb597-126">Properties</span></span>
| <span data-ttu-id="eb597-127">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb597-127">Property</span></span>     | <span data-ttu-id="eb597-128">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb597-128">Type</span></span>        | <span data-ttu-id="eb597-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb597-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb597-130">displayName</span><span class="sxs-lookup"><span data-stu-id="eb597-130">displayName</span></span>|<span data-ttu-id="eb597-131">String</span><span class="sxs-lookup"><span data-stu-id="eb597-131">String</span></span>|<span data-ttu-id="eb597-132">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="eb597-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="eb597-133">id</span><span class="sxs-lookup"><span data-stu-id="eb597-133">id</span></span>|<span data-ttu-id="eb597-134">String</span><span class="sxs-lookup"><span data-stu-id="eb597-134">String</span></span>| <span data-ttu-id="eb597-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb597-135">Read-only.</span></span>|
|<span data-ttu-id="eb597-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="eb597-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="eb597-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb597-137">Boolean</span></span>|<span data-ttu-id="eb597-138">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="eb597-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb597-139">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="eb597-139">Relationships</span></span>
| <span data-ttu-id="eb597-140">Relação</span><span class="sxs-lookup"><span data-stu-id="eb597-140">Relationship</span></span> | <span data-ttu-id="eb597-141">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb597-141">Type</span></span>        | <span data-ttu-id="eb597-142">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb597-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="eb597-143">arquivos</span><span class="sxs-lookup"><span data-stu-id="eb597-143">files</span></span>|<span data-ttu-id="eb597-144">coleção [agreementFile](agreementfile.md)</span><span class="sxs-lookup"><span data-stu-id="eb597-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="eb597-145">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb597-145">Read-only.</span></span> <span data-ttu-id="eb597-146">PDFs vinculada a este contrato.</span><span class="sxs-lookup"><span data-stu-id="eb597-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eb597-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb597-147">JSON representation</span></span>

<span data-ttu-id="eb597-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb597-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
