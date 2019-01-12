---
title: Tipo de recurso contact
description: Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 326c967f7cca9a24346ade36b96aa5878cb2d7ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915673"
---
# <a name="contract-resource-type"></a><span data-ttu-id="c8dad-103">Tipo de recurso contact</span><span class="sxs-lookup"><span data-stu-id="c8dad-103">Contract resource type</span></span>

> <span data-ttu-id="c8dad-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c8dad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8dad-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c8dad-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c8dad-106">Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="c8dad-106">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="c8dad-p102">**Importante:** Existe apenas em locatários do parceiro. Locatários do parceiro são locatários Azure AD que pertencem a parceiros da Microsoft que fazem parte do [Provedor de Soluções do Microsoft Cloud](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication ou programas de parceiro Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="c8dad-p102">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="c8dad-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c8dad-109">Methods</span></span>

| <span data-ttu-id="c8dad-110">Método</span><span class="sxs-lookup"><span data-stu-id="c8dad-110">Method</span></span>   | <span data-ttu-id="c8dad-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="c8dad-111">Return Type</span></span> | <span data-ttu-id="c8dad-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8dad-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="c8dad-113">Get contract</span><span class="sxs-lookup"><span data-stu-id="c8dad-113">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="c8dad-114">Contrato</span><span class="sxs-lookup"><span data-stu-id="c8dad-114">Contract</span></span> |<span data-ttu-id="c8dad-115">Ler propriedades de um objeto de contrato específico.</span><span class="sxs-lookup"><span data-stu-id="c8dad-115">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="c8dad-116">List contracts</span><span class="sxs-lookup"><span data-stu-id="c8dad-116">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="c8dad-117">Coleção de contratos</span><span class="sxs-lookup"><span data-stu-id="c8dad-117">Contract collection</span></span> | <span data-ttu-id="c8dad-118">Lista de contratos no locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="c8dad-118">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="c8dad-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8dad-119">Properties</span></span>
| <span data-ttu-id="c8dad-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8dad-120">Property</span></span>   | <span data-ttu-id="c8dad-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8dad-121">Type</span></span> | <span data-ttu-id="c8dad-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8dad-122">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c8dad-123">contractType</span><span class="sxs-lookup"><span data-stu-id="c8dad-123">contractType</span></span>|<span data-ttu-id="c8dad-124">String</span><span class="sxs-lookup"><span data-stu-id="c8dad-124">String</span></span>|<span data-ttu-id="c8dad-125">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="c8dad-125">Type of contract.</span></span><br><br><span data-ttu-id="c8dad-126">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="c8dad-126">Possible values are:</span></span><br> <span data-ttu-id="c8dad-p103">*SyndicationPartner* – parceiro que revende ou gerencia com exclusividade O365 e Intune para esse cliente. Eles revendem e oferecem suporte aos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="c8dad-p103">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="c8dad-p104">*BreadthPartner* – parceiro tem a capacidade de fornecer suporte administrativo para esse cliente. No entanto, o parceiro não tem permissão para revender ao cliente.</span><span class="sxs-lookup"><span data-stu-id="c8dad-p104">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="c8dad-p105">*ResellerPartner* – parceiro que é semelhante a um parceiro de agregação, exceto que o parceiro não tem acesso exclusivo ao locatário. No caso de agregação, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="c8dad-p105">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="c8dad-133">customerId</span><span class="sxs-lookup"><span data-stu-id="c8dad-133">customerId</span></span>|<span data-ttu-id="c8dad-134">Guid</span><span class="sxs-lookup"><span data-stu-id="c8dad-134">Guid</span></span>|<span data-ttu-id="c8dad-p106">O identificador exclusivo para o locatário de cliente referenciado por essa parceria. Corresponde à propriedade de identificação do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="c8dad-p106">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="c8dad-137">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="c8dad-137">defaultDomainName</span></span>|<span data-ttu-id="c8dad-138">String</span><span class="sxs-lookup"><span data-stu-id="c8dad-138">String</span></span>|<span data-ttu-id="c8dad-p107">Uma cópia do nome de domínio padrão do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="c8dad-p107">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="c8dad-142">displayName</span><span class="sxs-lookup"><span data-stu-id="c8dad-142">displayName</span></span>|<span data-ttu-id="c8dad-143">String</span><span class="sxs-lookup"><span data-stu-id="c8dad-143">String</span></span>|<span data-ttu-id="c8dad-p108">Uma cópia do nome de exibição do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de exibição do locatário do cliente é alterado.</span><span class="sxs-lookup"><span data-stu-id="c8dad-p108">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="c8dad-147">id</span><span class="sxs-lookup"><span data-stu-id="c8dad-147">id</span></span>|<span data-ttu-id="c8dad-148">String</span><span class="sxs-lookup"><span data-stu-id="c8dad-148">String</span></span>| <span data-ttu-id="c8dad-p109">O identificador exclusivo da parceria. Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="c8dad-p109">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="c8dad-151">Relações</span><span class="sxs-lookup"><span data-stu-id="c8dad-151">Relationships</span></span>
<span data-ttu-id="c8dad-152">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8dad-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c8dad-153">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8dad-153">JSON representation</span></span>
<span data-ttu-id="c8dad-154">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8dad-154">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
