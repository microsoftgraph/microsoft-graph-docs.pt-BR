---
title: Tipo de recurso de contrato
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: d1c573b43587ef5213f876b6532358fe5465f84b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962637"
---
# <a name="contract-resource-type"></a><span data-ttu-id="626dc-103">Tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="626dc-103">Contract resource type</span></span>

<span data-ttu-id="626dc-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="626dc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="626dc-105">Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="626dc-105">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="626dc-106">**Importante:** Existe apenas em locatários parceiros.</span><span class="sxs-lookup"><span data-stu-id="626dc-106">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="626dc-107">Os locatários de parceiros são locatários do Azure AD que pertencem aos parceiros da Microsoft que fazem parte do [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), do Office 365 Syndication ou dos programas de parceiros do Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="626dc-107">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="626dc-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="626dc-108">Methods</span></span>

| <span data-ttu-id="626dc-109">Método</span><span class="sxs-lookup"><span data-stu-id="626dc-109">Method</span></span>   | <span data-ttu-id="626dc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="626dc-110">Return Type</span></span> | <span data-ttu-id="626dc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="626dc-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="626dc-112">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="626dc-112">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="626dc-113">Contrato</span><span class="sxs-lookup"><span data-stu-id="626dc-113">Contract</span></span> |<span data-ttu-id="626dc-114">Ler propriedades de um objeto de contrato específico.</span><span class="sxs-lookup"><span data-stu-id="626dc-114">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="626dc-115">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="626dc-115">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="626dc-116">Coleção Contract</span><span class="sxs-lookup"><span data-stu-id="626dc-116">Contract collection</span></span> | <span data-ttu-id="626dc-117">Lista de contratos no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="626dc-117">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="626dc-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="626dc-118">Properties</span></span>
| <span data-ttu-id="626dc-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="626dc-119">Property</span></span>   | <span data-ttu-id="626dc-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="626dc-120">Type</span></span> | <span data-ttu-id="626dc-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="626dc-121">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="626dc-122">contractType</span><span class="sxs-lookup"><span data-stu-id="626dc-122">contractType</span></span>|<span data-ttu-id="626dc-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="626dc-123">String</span></span>|<span data-ttu-id="626dc-124">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="626dc-124">Type of contract.</span></span> <span data-ttu-id="626dc-125">Os valores possíveis são:  `SyndicationPartner` , `BreadthPartner` , `ResellerPartner` .</span><span class="sxs-lookup"><span data-stu-id="626dc-125">Possible values are:  `SyndicationPartner`, `BreadthPartner`, `ResellerPartner`.</span></span> <span data-ttu-id="626dc-126">Veja mais na [tabela abaixo](#contracttype-values).</span><span class="sxs-lookup"><span data-stu-id="626dc-126">See more in the [table below](#contracttype-values).</span></span> |
|<span data-ttu-id="626dc-127">customerId</span><span class="sxs-lookup"><span data-stu-id="626dc-127">customerId</span></span>|<span data-ttu-id="626dc-128">Guid</span><span class="sxs-lookup"><span data-stu-id="626dc-128">Guid</span></span>|<span data-ttu-id="626dc-129">O identificador exclusivo do locatário do cliente referenciado por essa parceria.</span><span class="sxs-lookup"><span data-stu-id="626dc-129">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="626dc-130">Corresponde à propriedade id do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="626dc-130">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="626dc-131">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="626dc-131">defaultDomainName</span></span>|<span data-ttu-id="626dc-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="626dc-132">String</span></span>|<span data-ttu-id="626dc-133">Uma cópia do nome de domínio padrão do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="626dc-133">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="626dc-134">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="626dc-134">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="626dc-135">Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente mudar.</span><span class="sxs-lookup"><span data-stu-id="626dc-135">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="626dc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="626dc-136">displayName</span></span>|<span data-ttu-id="626dc-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="626dc-137">String</span></span>|<span data-ttu-id="626dc-138">Uma cópia do nome de exibição do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="626dc-138">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="626dc-139">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="626dc-139">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="626dc-140">Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente mudar.</span><span class="sxs-lookup"><span data-stu-id="626dc-140">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="626dc-141">id</span><span class="sxs-lookup"><span data-stu-id="626dc-141">id</span></span>|<span data-ttu-id="626dc-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="626dc-142">String</span></span>| <span data-ttu-id="626dc-143">O identificador exclusivo da parceria.</span><span class="sxs-lookup"><span data-stu-id="626dc-143">The unique identifier for the partnership.</span></span> <span data-ttu-id="626dc-144">Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="626dc-144">Key, read-only</span></span> |

### <a name="contracttype-values"></a><span data-ttu-id="626dc-145">valores contractType</span><span class="sxs-lookup"><span data-stu-id="626dc-145">contractType values</span></span>

|<span data-ttu-id="626dc-146">Member</span><span class="sxs-lookup"><span data-stu-id="626dc-146">Member</span></span>|<span data-ttu-id="626dc-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="626dc-147">Description</span></span>|
|:---|:---|
|<span data-ttu-id="626dc-148">SyndicationPartner</span><span class="sxs-lookup"><span data-stu-id="626dc-148">SyndicationPartner</span></span>|<span data-ttu-id="626dc-149">Parceiro que *revende* e gerencia exclusivamente o O365 e o Intune para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="626dc-149">Partner that *exclusively* resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="626dc-150">Eles revendem e suportam seus clientes.</span><span class="sxs-lookup"><span data-stu-id="626dc-150">They resell and support their customers.</span></span>|
|<span data-ttu-id="626dc-151">BreadthPartner</span><span class="sxs-lookup"><span data-stu-id="626dc-151">BreadthPartner</span></span>|<span data-ttu-id="626dc-152">O parceiro tem a capacidade de fornecer suporte administrativo para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="626dc-152">Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="626dc-153">No entanto, o parceiro não tem permissão para revender para o cliente.</span><span class="sxs-lookup"><span data-stu-id="626dc-153">However, the partner is not allowed to resell to the customer.</span></span>|
|<span data-ttu-id="626dc-154">ResellerPartner</span><span class="sxs-lookup"><span data-stu-id="626dc-154">ResellerPartner</span></span>|<span data-ttu-id="626dc-155">Parceiro semelhante a um parceiro de sindicalidade, exceto que o parceiro não tem acesso exclusivo a um locatário.</span><span class="sxs-lookup"><span data-stu-id="626dc-155">Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="626dc-156">No caso de sindicalização, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="626dc-156">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|

## <a name="relationships"></a><span data-ttu-id="626dc-157">Relações</span><span class="sxs-lookup"><span data-stu-id="626dc-157">Relationships</span></span>
<span data-ttu-id="626dc-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="626dc-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="626dc-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="626dc-159">JSON representation</span></span>
<span data-ttu-id="626dc-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="626dc-160">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
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
<!--
{
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


