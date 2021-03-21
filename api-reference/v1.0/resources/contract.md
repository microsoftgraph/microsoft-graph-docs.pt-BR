---
title: Tipo de recurso de contrato
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 2ec65433edf3a6d0ec5973c0a3bc8cf46cef00d0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962466"
---
# <a name="contract-resource-type"></a><span data-ttu-id="15cc3-103">Tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="15cc3-103">Contract resource type</span></span>

<span data-ttu-id="15cc3-104">Namespace: microsoft.graph Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="15cc3-104">Namespace: microsoft.graph Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="15cc3-105">**Importante:** Existe apenas em locatários parceiros.</span><span class="sxs-lookup"><span data-stu-id="15cc3-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="15cc3-106">Os locatários de parceiros são locatários do Azure AD que pertencem aos parceiros da Microsoft que fazem parte do [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), do Office 365 Syndication ou dos programas de parceiros do Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="15cc3-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="15cc3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="15cc3-107">Methods</span></span>

| <span data-ttu-id="15cc3-108">Método</span><span class="sxs-lookup"><span data-stu-id="15cc3-108">Method</span></span>   | <span data-ttu-id="15cc3-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="15cc3-109">Return Type</span></span> | <span data-ttu-id="15cc3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="15cc3-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="15cc3-111">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="15cc3-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="15cc3-112">Contrato</span><span class="sxs-lookup"><span data-stu-id="15cc3-112">Contract</span></span> |<span data-ttu-id="15cc3-113">Ler propriedades de um objeto de contrato específico.</span><span class="sxs-lookup"><span data-stu-id="15cc3-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="15cc3-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="15cc3-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="15cc3-115">Coleção Contract</span><span class="sxs-lookup"><span data-stu-id="15cc3-115">Contract collection</span></span> | <span data-ttu-id="15cc3-116">Lista de contratos no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="15cc3-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="15cc3-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15cc3-117">Properties</span></span>
| <span data-ttu-id="15cc3-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15cc3-118">Property</span></span>   | <span data-ttu-id="15cc3-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="15cc3-119">Type</span></span> | <span data-ttu-id="15cc3-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="15cc3-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="15cc3-121">contractType</span><span class="sxs-lookup"><span data-stu-id="15cc3-121">contractType</span></span>|<span data-ttu-id="15cc3-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15cc3-122">String</span></span>|<span data-ttu-id="15cc3-123">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="15cc3-123">Type of contract.</span></span> <span data-ttu-id="15cc3-124">Os valores possíveis são:  `SyndicationPartner` , `BreadthPartner` , `ResellerPartner` .</span><span class="sxs-lookup"><span data-stu-id="15cc3-124">Possible values are:  `SyndicationPartner`, `BreadthPartner`, `ResellerPartner`.</span></span> <span data-ttu-id="15cc3-125">Veja mais na [tabela abaixo](#contracttype-values).</span><span class="sxs-lookup"><span data-stu-id="15cc3-125">See more in the [table below](#contracttype-values).</span></span>|
|<span data-ttu-id="15cc3-126">customerId</span><span class="sxs-lookup"><span data-stu-id="15cc3-126">customerId</span></span>|<span data-ttu-id="15cc3-127">Guid</span><span class="sxs-lookup"><span data-stu-id="15cc3-127">Guid</span></span>|<span data-ttu-id="15cc3-128">O identificador exclusivo do locatário do cliente referenciado por essa parceria.</span><span class="sxs-lookup"><span data-stu-id="15cc3-128">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="15cc3-129">Corresponde à propriedade id do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="15cc3-129">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="15cc3-130">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="15cc3-130">defaultDomainName</span></span>|<span data-ttu-id="15cc3-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15cc3-131">String</span></span>|<span data-ttu-id="15cc3-132">Uma cópia do nome de domínio padrão do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="15cc3-132">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="15cc3-133">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="15cc3-133">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="15cc3-134">Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente mudar.</span><span class="sxs-lookup"><span data-stu-id="15cc3-134">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="15cc3-135">displayName</span><span class="sxs-lookup"><span data-stu-id="15cc3-135">displayName</span></span>|<span data-ttu-id="15cc3-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15cc3-136">String</span></span>|<span data-ttu-id="15cc3-137">Uma cópia do nome de exibição do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="15cc3-137">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="15cc3-138">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="15cc3-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="15cc3-139">Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente mudar.</span><span class="sxs-lookup"><span data-stu-id="15cc3-139">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="15cc3-140">id</span><span class="sxs-lookup"><span data-stu-id="15cc3-140">id</span></span>|<span data-ttu-id="15cc3-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15cc3-141">String</span></span>| <span data-ttu-id="15cc3-142">O identificador exclusivo da parceria.</span><span class="sxs-lookup"><span data-stu-id="15cc3-142">The unique identifier for the partnership.</span></span> <span data-ttu-id="15cc3-143">Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="15cc3-143">Key, read-only</span></span> |

### <a name="contracttype-values"></a><span data-ttu-id="15cc3-144">valores contractType</span><span class="sxs-lookup"><span data-stu-id="15cc3-144">contractType values</span></span>

|<span data-ttu-id="15cc3-145">Member</span><span class="sxs-lookup"><span data-stu-id="15cc3-145">Member</span></span>|<span data-ttu-id="15cc3-146">Descrição</span><span class="sxs-lookup"><span data-stu-id="15cc3-146">Description</span></span>|
|:---|:---|
|<span data-ttu-id="15cc3-147">SyndicationPartner</span><span class="sxs-lookup"><span data-stu-id="15cc3-147">SyndicationPartner</span></span>|<span data-ttu-id="15cc3-148">Parceiro que *revende* e gerencia exclusivamente o O365 e o Intune para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="15cc3-148">Partner that *exclusively* resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="15cc3-149">Eles revendem e suportam seus clientes.</span><span class="sxs-lookup"><span data-stu-id="15cc3-149">They resell and support their customers.</span></span>|
|<span data-ttu-id="15cc3-150">BreadthPartner</span><span class="sxs-lookup"><span data-stu-id="15cc3-150">BreadthPartner</span></span>|<span data-ttu-id="15cc3-151">O parceiro tem a capacidade de fornecer suporte administrativo para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="15cc3-151">Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="15cc3-152">No entanto, o parceiro não tem permissão para revender para o cliente.</span><span class="sxs-lookup"><span data-stu-id="15cc3-152">However, the partner is not allowed to resell to the customer.</span></span>|
|<span data-ttu-id="15cc3-153">ResellerPartner</span><span class="sxs-lookup"><span data-stu-id="15cc3-153">ResellerPartner</span></span>|<span data-ttu-id="15cc3-154">Parceiro semelhante a um parceiro de sindicalidade, exceto que o parceiro não tem acesso exclusivo a um locatário.</span><span class="sxs-lookup"><span data-stu-id="15cc3-154">Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="15cc3-155">No caso de sindicalização, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="15cc3-155">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15cc3-156">Relações</span><span class="sxs-lookup"><span data-stu-id="15cc3-156">Relationships</span></span>
<span data-ttu-id="15cc3-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15cc3-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="15cc3-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15cc3-158">JSON representation</span></span>
<span data-ttu-id="15cc3-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15cc3-159">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

