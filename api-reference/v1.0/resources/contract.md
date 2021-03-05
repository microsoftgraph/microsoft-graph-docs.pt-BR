---
title: Tipo de recurso de contrato
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 35e8cbc38fd183907c09b26c05d5c95cc140a7f5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444424"
---
# <a name="contract-resource-type"></a><span data-ttu-id="dd68b-103">Tipo de recurso de contrato</span><span class="sxs-lookup"><span data-stu-id="dd68b-103">Contract resource type</span></span>

<span data-ttu-id="dd68b-104">Namespace: microsoft.graph Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="dd68b-104">Namespace: microsoft.graph Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="dd68b-105">**Importante:** Existe apenas em locatários parceiros.</span><span class="sxs-lookup"><span data-stu-id="dd68b-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="dd68b-106">Os locatários de parceiros são locatários do Azure AD que pertencem aos parceiros da Microsoft que fazem parte do [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), do Office 365 Syndication ou dos programas de parceiros do Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="dd68b-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="dd68b-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="dd68b-107">Methods</span></span>

| <span data-ttu-id="dd68b-108">Método</span><span class="sxs-lookup"><span data-stu-id="dd68b-108">Method</span></span>   | <span data-ttu-id="dd68b-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dd68b-109">Return Type</span></span> | <span data-ttu-id="dd68b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd68b-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd68b-111">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="dd68b-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="dd68b-112">Contrato</span><span class="sxs-lookup"><span data-stu-id="dd68b-112">Contract</span></span> |<span data-ttu-id="dd68b-113">Ler propriedades de um objeto de contrato específico.</span><span class="sxs-lookup"><span data-stu-id="dd68b-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="dd68b-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="dd68b-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="dd68b-115">Coleção Contract</span><span class="sxs-lookup"><span data-stu-id="dd68b-115">Contract collection</span></span> | <span data-ttu-id="dd68b-116">Lista de contratos no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="dd68b-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd68b-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dd68b-117">Properties</span></span>
| <span data-ttu-id="dd68b-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dd68b-118">Property</span></span>   | <span data-ttu-id="dd68b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="dd68b-119">Type</span></span> | <span data-ttu-id="dd68b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="dd68b-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="dd68b-121">contractType</span><span class="sxs-lookup"><span data-stu-id="dd68b-121">contractType</span></span>|<span data-ttu-id="dd68b-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd68b-122">String</span></span>|<span data-ttu-id="dd68b-123">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="dd68b-123">Type of contract.</span></span><br><br><span data-ttu-id="dd68b-124">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="dd68b-124">Possible values are:</span></span><br> <span data-ttu-id="dd68b-125">*SyndicationPartner* - Parceiro que revende e gerencia exclusivamente o O365 e o Intune para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="dd68b-125">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="dd68b-126">Eles revendem e suportam seus clientes.</span><span class="sxs-lookup"><span data-stu-id="dd68b-126">They resell and support their customers.</span></span><br> <span data-ttu-id="dd68b-127">*BreadthPartner* - O parceiro tem a capacidade de fornecer suporte administrativo para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="dd68b-127">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="dd68b-128">No entanto, o parceiro não tem permissão para revender para o cliente.</span><span class="sxs-lookup"><span data-stu-id="dd68b-128">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="dd68b-129">*ResellerPartner* - Parceiro semelhante a um parceiro de sindicalidade, exceto que o parceiro não tem acesso exclusivo a um locatário.</span><span class="sxs-lookup"><span data-stu-id="dd68b-129">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="dd68b-130">No caso de sindicalização, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="dd68b-130">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="dd68b-131">customerId</span><span class="sxs-lookup"><span data-stu-id="dd68b-131">customerId</span></span>|<span data-ttu-id="dd68b-132">Guid</span><span class="sxs-lookup"><span data-stu-id="dd68b-132">Guid</span></span>|<span data-ttu-id="dd68b-133">O identificador exclusivo do locatário do cliente referenciado por essa parceria.</span><span class="sxs-lookup"><span data-stu-id="dd68b-133">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="dd68b-134">Corresponde à propriedade id do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="dd68b-134">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="dd68b-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="dd68b-135">defaultDomainName</span></span>|<span data-ttu-id="dd68b-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd68b-136">String</span></span>|<span data-ttu-id="dd68b-137">Uma cópia do nome de domínio padrão do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="dd68b-137">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="dd68b-138">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="dd68b-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="dd68b-139">Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente mudar.</span><span class="sxs-lookup"><span data-stu-id="dd68b-139">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="dd68b-140">displayName</span><span class="sxs-lookup"><span data-stu-id="dd68b-140">displayName</span></span>|<span data-ttu-id="dd68b-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd68b-141">String</span></span>|<span data-ttu-id="dd68b-142">Uma cópia do nome de exibição do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="dd68b-142">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="dd68b-143">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="dd68b-143">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="dd68b-144">Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente mudar.</span><span class="sxs-lookup"><span data-stu-id="dd68b-144">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="dd68b-145">id</span><span class="sxs-lookup"><span data-stu-id="dd68b-145">id</span></span>|<span data-ttu-id="dd68b-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dd68b-146">String</span></span>| <span data-ttu-id="dd68b-147">O identificador exclusivo da parceria.</span><span class="sxs-lookup"><span data-stu-id="dd68b-147">The unique identifier for the partnership.</span></span> <span data-ttu-id="dd68b-148">Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="dd68b-148">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="dd68b-149">Relações</span><span class="sxs-lookup"><span data-stu-id="dd68b-149">Relationships</span></span>
<span data-ttu-id="dd68b-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dd68b-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="dd68b-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dd68b-151">JSON representation</span></span>
<span data-ttu-id="dd68b-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dd68b-152">Here is a JSON representation of the resource.</span></span>

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

