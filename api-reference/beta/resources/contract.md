---
title: Tipo de recurso Contract
description: Representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 67e2a4f78e33748b7648dd57892831faf7e27c23
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507419"
---
# <a name="contract-resource-type"></a><span data-ttu-id="8044f-103">Tipo de recurso Contract</span><span class="sxs-lookup"><span data-stu-id="8044f-103">Contract resource type</span></span>

<span data-ttu-id="8044f-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8044f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8044f-105">Representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="8044f-105">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="8044f-106">**Importante:** Existe somente nos locatários do parceiro.</span><span class="sxs-lookup"><span data-stu-id="8044f-106">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="8044f-107">Os locatários de parceiros são locatários do Azure AD que pertencem a parceiros da Microsoft que fazem parte do [provedor de soluções de nuvem da Microsoft](https://partnercenter.microsoft.com/en-us/partner/programs), da distribuição do Office 365 ou dos programas de parceria do Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="8044f-107">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="8044f-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8044f-108">Methods</span></span>

| <span data-ttu-id="8044f-109">Método</span><span class="sxs-lookup"><span data-stu-id="8044f-109">Method</span></span>   | <span data-ttu-id="8044f-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8044f-110">Return Type</span></span> | <span data-ttu-id="8044f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8044f-111">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="8044f-112">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="8044f-112">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="8044f-113">Contrato</span><span class="sxs-lookup"><span data-stu-id="8044f-113">Contract</span></span> |<span data-ttu-id="8044f-114">Ler as propriedades de um objeto Contract específico.</span><span class="sxs-lookup"><span data-stu-id="8044f-114">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="8044f-115">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="8044f-115">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="8044f-116">Coleção Contract</span><span class="sxs-lookup"><span data-stu-id="8044f-116">Contract collection</span></span> | <span data-ttu-id="8044f-117">Lista de contratos no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="8044f-117">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="8044f-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8044f-118">Properties</span></span>
| <span data-ttu-id="8044f-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8044f-119">Property</span></span>   | <span data-ttu-id="8044f-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="8044f-120">Type</span></span> | <span data-ttu-id="8044f-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="8044f-121">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8044f-122">ContractType</span><span class="sxs-lookup"><span data-stu-id="8044f-122">contractType</span></span>|<span data-ttu-id="8044f-123">String</span><span class="sxs-lookup"><span data-stu-id="8044f-123">String</span></span>|<span data-ttu-id="8044f-124">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="8044f-124">Type of contract.</span></span><br><br><span data-ttu-id="8044f-125">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="8044f-125">Possible values are:</span></span><br> <span data-ttu-id="8044f-126">*SyndicationPartner* -parceiro que revende exclusivamente e gerencia o O365 e o Intune para este cliente.</span><span class="sxs-lookup"><span data-stu-id="8044f-126">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="8044f-127">Eles revendem e dão suporte a seus clientes.</span><span class="sxs-lookup"><span data-stu-id="8044f-127">They resell and support their customers.</span></span><br> <span data-ttu-id="8044f-128">*BreadthPartner* -o parceiro tem a capacidade de fornecer suporte administrativo para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="8044f-128">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="8044f-129">No entanto, o parceiro não tem permissão para revender para o cliente.</span><span class="sxs-lookup"><span data-stu-id="8044f-129">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="8044f-130">*ResellerPartner* -Partner que é semelhante a um parceiro de distribuição, exceto pelo fato de que o parceiro não tem acesso exclusivo a um locatário.</span><span class="sxs-lookup"><span data-stu-id="8044f-130">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="8044f-131">No caso de distribuição, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="8044f-131">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="8044f-132">Box</span><span class="sxs-lookup"><span data-stu-id="8044f-132">customerId</span></span>|<span data-ttu-id="8044f-133">Guid</span><span class="sxs-lookup"><span data-stu-id="8044f-133">Guid</span></span>|<span data-ttu-id="8044f-134">O identificador exclusivo do locatário do cliente referido por esta parceria.</span><span class="sxs-lookup"><span data-stu-id="8044f-134">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="8044f-135">Corresponde à propriedade ID do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="8044f-135">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="8044f-136">DefaultDomainName</span><span class="sxs-lookup"><span data-stu-id="8044f-136">defaultDomainName</span></span>|<span data-ttu-id="8044f-137">String</span><span class="sxs-lookup"><span data-stu-id="8044f-137">String</span></span>|<span data-ttu-id="8044f-138">Uma cópia do nome de domínio padrão do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="8044f-138">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="8044f-139">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="8044f-139">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="8044f-140">Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="8044f-140">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="8044f-141">displayName</span><span class="sxs-lookup"><span data-stu-id="8044f-141">displayName</span></span>|<span data-ttu-id="8044f-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8044f-142">String</span></span>|<span data-ttu-id="8044f-143">Uma cópia do nome de exibição do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="8044f-143">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="8044f-144">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="8044f-144">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="8044f-145">Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="8044f-145">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="8044f-146">id</span><span class="sxs-lookup"><span data-stu-id="8044f-146">id</span></span>|<span data-ttu-id="8044f-147">String</span><span class="sxs-lookup"><span data-stu-id="8044f-147">String</span></span>| <span data-ttu-id="8044f-148">O identificador exclusivo da parceria.</span><span class="sxs-lookup"><span data-stu-id="8044f-148">The unique identifier for the partnership.</span></span> <span data-ttu-id="8044f-149">Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="8044f-149">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="8044f-150">Relações</span><span class="sxs-lookup"><span data-stu-id="8044f-150">Relationships</span></span>
<span data-ttu-id="8044f-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8044f-151">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8044f-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8044f-152">JSON representation</span></span>
<span data-ttu-id="8044f-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8044f-153">Here is a JSON representation of the resource.</span></span>

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
