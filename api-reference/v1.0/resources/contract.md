---
title: Tipo de recurso contact
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
ms.openlocfilehash: 5058ea32946df677596dfb0e4502c6f9d4145ec2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003577"
---
# <a name="contract-resource-type"></a><span data-ttu-id="2a77e-103">Tipo de recurso contact</span><span class="sxs-lookup"><span data-stu-id="2a77e-103">Contract resource type</span></span>
<span data-ttu-id="2a77e-104">Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="2a77e-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="2a77e-p101">**Importante:** Existe apenas em locatários do parceiro. Locatários do parceiro são locatários Azure AD que pertencem a parceiros da Microsoft que fazem parte do [Provedor de Soluções do Microsoft Cloud](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication ou programas de parceiro Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="2a77e-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="2a77e-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="2a77e-107">Methods</span></span>

| <span data-ttu-id="2a77e-108">Método</span><span class="sxs-lookup"><span data-stu-id="2a77e-108">Method</span></span>   | <span data-ttu-id="2a77e-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="2a77e-109">Return Type</span></span> | <span data-ttu-id="2a77e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a77e-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="2a77e-111">Get contract</span><span class="sxs-lookup"><span data-stu-id="2a77e-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="2a77e-112">Contrato</span><span class="sxs-lookup"><span data-stu-id="2a77e-112">Contract</span></span> |<span data-ttu-id="2a77e-113">Ler propriedades de um objeto de contrato específico.</span><span class="sxs-lookup"><span data-stu-id="2a77e-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="2a77e-114">List contracts</span><span class="sxs-lookup"><span data-stu-id="2a77e-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="2a77e-115">Coleção de contratos</span><span class="sxs-lookup"><span data-stu-id="2a77e-115">Contract collection</span></span> | <span data-ttu-id="2a77e-116">Lista de contratos no locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="2a77e-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="2a77e-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2a77e-117">Properties</span></span>
| <span data-ttu-id="2a77e-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2a77e-118">Property</span></span>   | <span data-ttu-id="2a77e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="2a77e-119">Type</span></span> | <span data-ttu-id="2a77e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a77e-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2a77e-121">contractType</span><span class="sxs-lookup"><span data-stu-id="2a77e-121">contractType</span></span>|<span data-ttu-id="2a77e-122">String</span><span class="sxs-lookup"><span data-stu-id="2a77e-122">String</span></span>|<span data-ttu-id="2a77e-123">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="2a77e-123">Type of contract.</span></span><br><br><span data-ttu-id="2a77e-124">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="2a77e-124">Possible values are:</span></span><br> <span data-ttu-id="2a77e-p102">*SyndicationPartner* – parceiro que revende ou gerencia com exclusividade O365 e Intune para esse cliente. Eles revendem e oferecem suporte aos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="2a77e-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="2a77e-p103">*BreadthPartner* – parceiro tem a capacidade de fornecer suporte administrativo para esse cliente. No entanto, o parceiro não tem permissão para revender ao cliente.</span><span class="sxs-lookup"><span data-stu-id="2a77e-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="2a77e-p104">*ResellerPartner* – parceiro que é semelhante a um parceiro de agregação, exceto que o parceiro não tem acesso exclusivo ao locatário. No caso de agregação, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="2a77e-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="2a77e-131">customerId</span><span class="sxs-lookup"><span data-stu-id="2a77e-131">customerId</span></span>|<span data-ttu-id="2a77e-132">Guid</span><span class="sxs-lookup"><span data-stu-id="2a77e-132">Guid</span></span>|<span data-ttu-id="2a77e-p105">O identificador exclusivo para o locatário de cliente referenciado por essa parceria. Corresponde à propriedade de identificação do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="2a77e-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="2a77e-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="2a77e-135">defaultDomainName</span></span>|<span data-ttu-id="2a77e-136">String</span><span class="sxs-lookup"><span data-stu-id="2a77e-136">String</span></span>|<span data-ttu-id="2a77e-p106">Uma cópia do nome de domínio padrão do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="2a77e-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="2a77e-140">displayName</span><span class="sxs-lookup"><span data-stu-id="2a77e-140">displayName</span></span>|<span data-ttu-id="2a77e-141">String</span><span class="sxs-lookup"><span data-stu-id="2a77e-141">String</span></span>|<span data-ttu-id="2a77e-p107">Uma cópia do nome de exibição do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de exibição do locatário do cliente é alterado.</span><span class="sxs-lookup"><span data-stu-id="2a77e-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="2a77e-145">id</span><span class="sxs-lookup"><span data-stu-id="2a77e-145">id</span></span>|<span data-ttu-id="2a77e-146">String</span><span class="sxs-lookup"><span data-stu-id="2a77e-146">String</span></span>| <span data-ttu-id="2a77e-p108">O identificador exclusivo da parceria. Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="2a77e-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="2a77e-149">Relações</span><span class="sxs-lookup"><span data-stu-id="2a77e-149">Relationships</span></span>
<span data-ttu-id="2a77e-150">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2a77e-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2a77e-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2a77e-151">JSON representation</span></span>
<span data-ttu-id="2a77e-152">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2a77e-152">Here is a JSON representation of the resource.</span></span>

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