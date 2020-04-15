---
title: Tipo de recurso Contract
description: Representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1086f1ebe43904074d0f6b99985637e7bb928fbf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449437"
---
# <a name="contract-resource-type"></a><span data-ttu-id="5fd75-103">Tipo de recurso Contract</span><span class="sxs-lookup"><span data-stu-id="5fd75-103">Contract resource type</span></span>

<span data-ttu-id="5fd75-104">Namespace: Microsoft. Graph representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fd75-104">Namespace: microsoft.graph Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="5fd75-105">**Importante:** Existe somente nos locatários do parceiro.</span><span class="sxs-lookup"><span data-stu-id="5fd75-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="5fd75-106">Os locatários de parceiros são locatários do Azure AD que pertencem a parceiros da Microsoft que fazem parte do [provedor de soluções de nuvem da Microsoft](https://partnercenter.microsoft.com/en-us/partner/programs), da distribuição do Office 365 ou dos programas de parceria do Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="5fd75-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="5fd75-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5fd75-107">Methods</span></span>

| <span data-ttu-id="5fd75-108">Método</span><span class="sxs-lookup"><span data-stu-id="5fd75-108">Method</span></span>   | <span data-ttu-id="5fd75-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5fd75-109">Return Type</span></span> | <span data-ttu-id="5fd75-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fd75-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="5fd75-111">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="5fd75-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="5fd75-112">Contrato</span><span class="sxs-lookup"><span data-stu-id="5fd75-112">Contract</span></span> |<span data-ttu-id="5fd75-113">Ler as propriedades de um objeto Contract específico.</span><span class="sxs-lookup"><span data-stu-id="5fd75-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="5fd75-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="5fd75-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="5fd75-115">Coleção Contract</span><span class="sxs-lookup"><span data-stu-id="5fd75-115">Contract collection</span></span> | <span data-ttu-id="5fd75-116">Lista de contratos no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="5fd75-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="5fd75-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fd75-117">Properties</span></span>
| <span data-ttu-id="5fd75-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fd75-118">Property</span></span>   | <span data-ttu-id="5fd75-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fd75-119">Type</span></span> | <span data-ttu-id="5fd75-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fd75-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5fd75-121">ContractType</span><span class="sxs-lookup"><span data-stu-id="5fd75-121">contractType</span></span>|<span data-ttu-id="5fd75-122">String</span><span class="sxs-lookup"><span data-stu-id="5fd75-122">String</span></span>|<span data-ttu-id="5fd75-123">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="5fd75-123">Type of contract.</span></span><br><br><span data-ttu-id="5fd75-124">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="5fd75-124">Possible values are:</span></span><br> <span data-ttu-id="5fd75-125">*SyndicationPartner* -parceiro que revende exclusivamente e gerencia o O365 e o Intune para este cliente.</span><span class="sxs-lookup"><span data-stu-id="5fd75-125">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="5fd75-126">Eles revendem e dão suporte a seus clientes.</span><span class="sxs-lookup"><span data-stu-id="5fd75-126">They resell and support their customers.</span></span><br> <span data-ttu-id="5fd75-127">*BreadthPartner* -o parceiro tem a capacidade de fornecer suporte administrativo para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="5fd75-127">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="5fd75-128">No entanto, o parceiro não tem permissão para revender para o cliente.</span><span class="sxs-lookup"><span data-stu-id="5fd75-128">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="5fd75-129">*ResellerPartner* -Partner que é semelhante a um parceiro de distribuição, exceto pelo fato de que o parceiro não tem acesso exclusivo a um locatário.</span><span class="sxs-lookup"><span data-stu-id="5fd75-129">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="5fd75-130">No caso de distribuição, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="5fd75-130">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="5fd75-131">Box</span><span class="sxs-lookup"><span data-stu-id="5fd75-131">customerId</span></span>|<span data-ttu-id="5fd75-132">Guid</span><span class="sxs-lookup"><span data-stu-id="5fd75-132">Guid</span></span>|<span data-ttu-id="5fd75-133">O identificador exclusivo do locatário do cliente referido por esta parceria.</span><span class="sxs-lookup"><span data-stu-id="5fd75-133">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="5fd75-134">Corresponde à propriedade ID do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fd75-134">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="5fd75-135">DefaultDomainName</span><span class="sxs-lookup"><span data-stu-id="5fd75-135">defaultDomainName</span></span>|<span data-ttu-id="5fd75-136">String</span><span class="sxs-lookup"><span data-stu-id="5fd75-136">String</span></span>|<span data-ttu-id="5fd75-137">Uma cópia do nome de domínio padrão do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fd75-137">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="5fd75-138">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="5fd75-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="5fd75-139">Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="5fd75-139">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="5fd75-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5fd75-140">displayName</span></span>|<span data-ttu-id="5fd75-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5fd75-141">String</span></span>|<span data-ttu-id="5fd75-142">Uma cópia do nome de exibição do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="5fd75-142">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="5fd75-143">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="5fd75-143">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="5fd75-144">Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="5fd75-144">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="5fd75-145">id</span><span class="sxs-lookup"><span data-stu-id="5fd75-145">id</span></span>|<span data-ttu-id="5fd75-146">String</span><span class="sxs-lookup"><span data-stu-id="5fd75-146">String</span></span>| <span data-ttu-id="5fd75-147">O identificador exclusivo da parceria.</span><span class="sxs-lookup"><span data-stu-id="5fd75-147">The unique identifier for the partnership.</span></span> <span data-ttu-id="5fd75-148">Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="5fd75-148">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="5fd75-149">Relações</span><span class="sxs-lookup"><span data-stu-id="5fd75-149">Relationships</span></span>
<span data-ttu-id="5fd75-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5fd75-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5fd75-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fd75-151">JSON representation</span></span>
<span data-ttu-id="5fd75-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5fd75-152">Here is a JSON representation of the resource.</span></span>

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
