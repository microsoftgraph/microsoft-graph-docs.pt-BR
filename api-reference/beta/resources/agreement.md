---
title: tipo de recurso de contrato
description: Representa os termos personalizável de um locatário contrato de uso que é criado e gerenciado com o Azure Active Directory (AD Azure). Você pode usar os métodos a seguir para criar e gerenciar o recurso do Windows Azure Active Directory termos de uso de acordo com o seu cenário.
ms.openlocfilehash: 2e5c9087cd809f9c067150654d420fda533ca61b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035469"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="012f7-104">tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="012f7-104">agreement resource type</span></span>

> <span data-ttu-id="012f7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="012f7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="012f7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="012f7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="012f7-107">Representa os termos personalizável de um locatário contrato de uso que é criado e gerenciado com o Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="012f7-107">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="012f7-108">Você pode usar os métodos a seguir para criar e gerenciar o [Azure Active Directory termos de uso de recurso](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) de acordo com seu cenário.</span><span class="sxs-lookup"><span data-stu-id="012f7-108">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="012f7-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="012f7-109">Methods</span></span>

| <span data-ttu-id="012f7-110">Método</span><span class="sxs-lookup"><span data-stu-id="012f7-110">Method</span></span>       | <span data-ttu-id="012f7-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="012f7-111">Return Type</span></span> | <span data-ttu-id="012f7-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="012f7-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="012f7-113">Criar contratos</span><span class="sxs-lookup"><span data-stu-id="012f7-113">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="012f7-114">contrato</span><span class="sxs-lookup"><span data-stu-id="012f7-114">agreement</span></span>](agreement.md) | <span data-ttu-id="012f7-115">Crie um novo contrato pelo lançamento à coleção contrato.</span><span class="sxs-lookup"><span data-stu-id="012f7-115">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="012f7-116">Contratos de lista</span><span class="sxs-lookup"><span data-stu-id="012f7-116">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="012f7-117">coleção de [contrato](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="012f7-117">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="012f7-118">Obtenha uma coleção de objetos do contrato.</span><span class="sxs-lookup"><span data-stu-id="012f7-118">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="012f7-119">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="012f7-119">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="012f7-120">contrato</span><span class="sxs-lookup"><span data-stu-id="012f7-120">agreement</span></span>](agreement.md) | <span data-ttu-id="012f7-121">Leia as propriedades e os relacionamentos de um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="012f7-121">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="012f7-122">Atualizar contrato</span><span class="sxs-lookup"><span data-stu-id="012f7-122">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="012f7-123">contrato</span><span class="sxs-lookup"><span data-stu-id="012f7-123">agreement</span></span>](agreement.md) | <span data-ttu-id="012f7-124">Atualize um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="012f7-124">Update an agreement object.</span></span> |
| [<span data-ttu-id="012f7-125">Excluir contrato</span><span class="sxs-lookup"><span data-stu-id="012f7-125">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="012f7-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="012f7-126">None</span></span> | <span data-ttu-id="012f7-127">Exclua um objeto de contrato.</span><span class="sxs-lookup"><span data-stu-id="012f7-127">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="012f7-128">Propriedades</span><span class="sxs-lookup"><span data-stu-id="012f7-128">Properties</span></span>
| <span data-ttu-id="012f7-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="012f7-129">Property</span></span>     | <span data-ttu-id="012f7-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="012f7-130">Type</span></span>        | <span data-ttu-id="012f7-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="012f7-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="012f7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="012f7-132">displayName</span></span>|<span data-ttu-id="012f7-133">String</span><span class="sxs-lookup"><span data-stu-id="012f7-133">String</span></span>|<span data-ttu-id="012f7-134">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="012f7-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="012f7-135">id</span><span class="sxs-lookup"><span data-stu-id="012f7-135">id</span></span>|<span data-ttu-id="012f7-136">String</span><span class="sxs-lookup"><span data-stu-id="012f7-136">String</span></span>| <span data-ttu-id="012f7-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="012f7-137">Read-only.</span></span>|
|<span data-ttu-id="012f7-138">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="012f7-138">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="012f7-139">Booliano</span><span class="sxs-lookup"><span data-stu-id="012f7-139">Boolean</span></span>|<span data-ttu-id="012f7-140">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="012f7-140">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="012f7-141">Relações</span><span class="sxs-lookup"><span data-stu-id="012f7-141">Relationships</span></span>
| <span data-ttu-id="012f7-142">Relação</span><span class="sxs-lookup"><span data-stu-id="012f7-142">Relationship</span></span> | <span data-ttu-id="012f7-143">Tipo</span><span class="sxs-lookup"><span data-stu-id="012f7-143">Type</span></span>        | <span data-ttu-id="012f7-144">Descrição</span><span class="sxs-lookup"><span data-stu-id="012f7-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="012f7-145">arquivos</span><span class="sxs-lookup"><span data-stu-id="012f7-145">files</span></span>|<span data-ttu-id="012f7-146">coleção [agreementFile](agreementfile.md)</span><span class="sxs-lookup"><span data-stu-id="012f7-146">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="012f7-147">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="012f7-147">Read-only.</span></span> <span data-ttu-id="012f7-148">PDFs vinculada a este contrato.</span><span class="sxs-lookup"><span data-stu-id="012f7-148">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="012f7-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="012f7-149">JSON representation</span></span>

<span data-ttu-id="012f7-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="012f7-150">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
