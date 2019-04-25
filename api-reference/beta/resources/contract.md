---
title: Tipo de recurso Contract
description: Representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6309dfc370d414ccb66065fe4048d7cece51f018
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535424"
---
# <a name="contract-resource-type"></a><span data-ttu-id="6cd15-103">Tipo de recurso Contract</span><span class="sxs-lookup"><span data-stu-id="6cd15-103">Contract resource type</span></span>
<span data-ttu-id="6cd15-104">Representa uma parceria existente que o locatário do parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="6cd15-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="6cd15-105">**Importante:** Existe somente nos locatários do parceiro.</span><span class="sxs-lookup"><span data-stu-id="6cd15-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="6cd15-106">Os locatários de parceiros são locatários do Azure AD que pertencem a parceiros da Microsoft que fazem parte do [provedor de soluções de nuvem da Microsoft](https://partnercenter.microsoft.com/en-us/partner/programs), da distribuição do Office 365 ou dos programas de parceria do Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="6cd15-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="6cd15-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6cd15-107">Methods</span></span>

| <span data-ttu-id="6cd15-108">Método</span><span class="sxs-lookup"><span data-stu-id="6cd15-108">Method</span></span>   | <span data-ttu-id="6cd15-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6cd15-109">Return Type</span></span> | <span data-ttu-id="6cd15-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cd15-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="6cd15-111">Obter contrato</span><span class="sxs-lookup"><span data-stu-id="6cd15-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="6cd15-112">Contrato</span><span class="sxs-lookup"><span data-stu-id="6cd15-112">Contract</span></span> |<span data-ttu-id="6cd15-113">Ler as propriedades de um objeto Contract específico.</span><span class="sxs-lookup"><span data-stu-id="6cd15-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="6cd15-114">Listar contratos</span><span class="sxs-lookup"><span data-stu-id="6cd15-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="6cd15-115">Coleção Contract</span><span class="sxs-lookup"><span data-stu-id="6cd15-115">Contract collection</span></span> | <span data-ttu-id="6cd15-116">Lista de contratos no locatário do parceiro.</span><span class="sxs-lookup"><span data-stu-id="6cd15-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="6cd15-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6cd15-117">Properties</span></span>
| <span data-ttu-id="6cd15-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6cd15-118">Property</span></span>   | <span data-ttu-id="6cd15-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6cd15-119">Type</span></span> | <span data-ttu-id="6cd15-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6cd15-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="6cd15-121">ContractType</span><span class="sxs-lookup"><span data-stu-id="6cd15-121">contractType</span></span>|<span data-ttu-id="6cd15-122">String</span><span class="sxs-lookup"><span data-stu-id="6cd15-122">String</span></span>|<span data-ttu-id="6cd15-123">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="6cd15-123">Type of contract.</span></span><br><br><span data-ttu-id="6cd15-124">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="6cd15-124">Possible values are:</span></span><br> <span data-ttu-id="6cd15-125">*SyndicationPartner* -parceiro que revende exclusivamente e gerencia o O365 e o Intune para este cliente.</span><span class="sxs-lookup"><span data-stu-id="6cd15-125">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="6cd15-126">Eles revendem e dão suporte a seus clientes.</span><span class="sxs-lookup"><span data-stu-id="6cd15-126">They resell and support their customers.</span></span><br> <span data-ttu-id="6cd15-127">*BreadthPartner* -o parceiro tem a capacidade de fornecer suporte administrativo para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="6cd15-127">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="6cd15-128">No enTanto, o parceiro não tem permissão para revender para o cliente.</span><span class="sxs-lookup"><span data-stu-id="6cd15-128">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="6cd15-129">*ResellerPartner* -Partner que é semelhante a um parceiro de distribuição, exceto pelo fato de que o parceiro não tem acesso exclusivo a um locatário.</span><span class="sxs-lookup"><span data-stu-id="6cd15-129">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="6cd15-130">No caso de distribuição, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="6cd15-130">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="6cd15-131">Box</span><span class="sxs-lookup"><span data-stu-id="6cd15-131">customerId</span></span>|<span data-ttu-id="6cd15-132">Guid</span><span class="sxs-lookup"><span data-stu-id="6cd15-132">Guid</span></span>|<span data-ttu-id="6cd15-133">O identificador exclusivo do locatário do cliente referido por esta parceria.</span><span class="sxs-lookup"><span data-stu-id="6cd15-133">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="6cd15-134">Corresponde à propriedade ID do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="6cd15-134">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="6cd15-135">defaultDomainname</span><span class="sxs-lookup"><span data-stu-id="6cd15-135">defaultDomainName</span></span>|<span data-ttu-id="6cd15-136">String</span><span class="sxs-lookup"><span data-stu-id="6cd15-136">String</span></span>|<span data-ttu-id="6cd15-137">Uma cópia do nome de domínio padrão do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="6cd15-137">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="6cd15-138">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="6cd15-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="6cd15-139">Ele não será atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="6cd15-139">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="6cd15-140">displayName</span><span class="sxs-lookup"><span data-stu-id="6cd15-140">displayName</span></span>|<span data-ttu-id="6cd15-141">String</span><span class="sxs-lookup"><span data-stu-id="6cd15-141">String</span></span>|<span data-ttu-id="6cd15-142">Uma cópia do nome de exibição do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="6cd15-142">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="6cd15-143">A cópia é feita quando a parceria com o cliente é estabelecida.</span><span class="sxs-lookup"><span data-stu-id="6cd15-143">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="6cd15-144">Ele não será atualizado automaticamente se o nome de exibição do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="6cd15-144">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="6cd15-145">id</span><span class="sxs-lookup"><span data-stu-id="6cd15-145">id</span></span>|<span data-ttu-id="6cd15-146">String</span><span class="sxs-lookup"><span data-stu-id="6cd15-146">String</span></span>| <span data-ttu-id="6cd15-147">O identificador exclusivo da parceria.</span><span class="sxs-lookup"><span data-stu-id="6cd15-147">The unique identifier for the partnership.</span></span> <span data-ttu-id="6cd15-148">Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="6cd15-148">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="6cd15-149">Relações</span><span class="sxs-lookup"><span data-stu-id="6cd15-149">Relationships</span></span>
<span data-ttu-id="6cd15-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6cd15-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6cd15-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6cd15-151">JSON representation</span></span>
<span data-ttu-id="6cd15-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6cd15-152">Here is a JSON representation of the resource.</span></span>

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
