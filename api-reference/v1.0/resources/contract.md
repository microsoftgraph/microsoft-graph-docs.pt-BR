# <a name="contract-resource-type"></a><span data-ttu-id="d5dae-101">Tipo de recurso contact</span><span class="sxs-lookup"><span data-stu-id="d5dae-101">Contract resource type</span></span>
<span data-ttu-id="d5dae-102">Representa uma parceria existente que o locatário parceiro tem com um locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="d5dae-102">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="d5dae-p101">**Importante:** Existe apenas em locatários do parceiro. Locatários do parceiro são locatários Azure AD que pertencem a parceiros da Microsoft que fazem parte do [Provedor de Soluções do Microsoft Cloud](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication ou programas de parceiro Microsoft Advisor.</span><span class="sxs-lookup"><span data-stu-id="d5dae-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="d5dae-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="d5dae-105">Methods</span></span>

| <span data-ttu-id="d5dae-106">Método</span><span class="sxs-lookup"><span data-stu-id="d5dae-106">Method</span></span>   | <span data-ttu-id="d5dae-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d5dae-107">Return Type</span></span> | <span data-ttu-id="d5dae-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5dae-108">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="d5dae-109">Get contract</span><span class="sxs-lookup"><span data-stu-id="d5dae-109">Get contract</span></span>](../api/contract_get.md) | <span data-ttu-id="d5dae-110">Contrato</span><span class="sxs-lookup"><span data-stu-id="d5dae-110">Contract</span></span> |<span data-ttu-id="d5dae-111">Ler propriedades de um objeto de contrato específico.</span><span class="sxs-lookup"><span data-stu-id="d5dae-111">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="d5dae-112">List contracts</span><span class="sxs-lookup"><span data-stu-id="d5dae-112">List contracts</span></span>](../api/contract_list.md) | <span data-ttu-id="d5dae-113">Coleção de contratos</span><span class="sxs-lookup"><span data-stu-id="d5dae-113">Contract collection</span></span> | <span data-ttu-id="d5dae-114">Lista de contratos no locatário parceiro.</span><span class="sxs-lookup"><span data-stu-id="d5dae-114">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="d5dae-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5dae-115">Properties</span></span>
| <span data-ttu-id="d5dae-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5dae-116">Property</span></span>   | <span data-ttu-id="d5dae-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5dae-117">Type</span></span> | <span data-ttu-id="d5dae-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5dae-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="d5dae-119">contractType</span><span class="sxs-lookup"><span data-stu-id="d5dae-119">contractType</span></span>|<span data-ttu-id="d5dae-120">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5dae-120">String</span></span>|<span data-ttu-id="d5dae-121">Tipo de contrato.</span><span class="sxs-lookup"><span data-stu-id="d5dae-121">Type of contract.</span></span><br><br><span data-ttu-id="d5dae-122">Os valores possíveis são:</span><span class="sxs-lookup"><span data-stu-id="d5dae-122">Possible values are:</span></span><br> <span data-ttu-id="d5dae-p102">*SyndicationPartner* – parceiro que revende ou gerencia com exclusividade O365 e Intune para esse cliente. Eles revendem e oferecem suporte aos seus clientes.</span><span class="sxs-lookup"><span data-stu-id="d5dae-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="d5dae-p103">*BreadthPartner* – parceiro tem a capacidade de fornecer suporte administrativo para esse cliente. No entanto, o parceiro não tem permissão para revender ao cliente.</span><span class="sxs-lookup"><span data-stu-id="d5dae-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="d5dae-p104">*ResellerPartner* – parceiro que é semelhante a um parceiro de agregação, exceto que o parceiro não tem acesso exclusivo ao locatário. No caso de agregação, o cliente não pode comprar assinaturas diretas adicionais da Microsoft ou de outros parceiros.</span><span class="sxs-lookup"><span data-stu-id="d5dae-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="d5dae-129">customerId</span><span class="sxs-lookup"><span data-stu-id="d5dae-129">customerId</span></span>|<span data-ttu-id="d5dae-130">Guid</span><span class="sxs-lookup"><span data-stu-id="d5dae-130">Guid</span></span>|<span data-ttu-id="d5dae-p105">O identificador exclusivo para o locatário de cliente referenciado por essa parceria. Corresponde à propriedade de identificação do recurso de organização do locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="d5dae-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="d5dae-133">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="d5dae-133">defaultDomainName</span></span>|<span data-ttu-id="d5dae-134">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5dae-134">String</span></span>|<span data-ttu-id="d5dae-p106">Uma cópia do nome de domínio padrão do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de domínio padrão do locatário do cliente for alterado.</span><span class="sxs-lookup"><span data-stu-id="d5dae-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="d5dae-138">displayName</span><span class="sxs-lookup"><span data-stu-id="d5dae-138">displayName</span></span>|<span data-ttu-id="d5dae-139">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5dae-139">String</span></span>|<span data-ttu-id="d5dae-p107">Uma cópia do nome de exibição do locatário do cliente. A cópia é feita quando a parceria com o cliente é estabelecida. Ele não é atualizado automaticamente se o nome de exibição do locatário do cliente é alterado.</span><span class="sxs-lookup"><span data-stu-id="d5dae-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="d5dae-143">id</span><span class="sxs-lookup"><span data-stu-id="d5dae-143">id</span></span>|<span data-ttu-id="d5dae-144">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5dae-144">String</span></span>| <span data-ttu-id="d5dae-p108">O identificador exclusivo da parceria. Chave, somente leitura</span><span class="sxs-lookup"><span data-stu-id="d5dae-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="d5dae-147">Relações</span><span class="sxs-lookup"><span data-stu-id="d5dae-147">Relationships</span></span>
<span data-ttu-id="d5dae-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d5dae-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d5dae-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5dae-149">JSON representation</span></span>
<span data-ttu-id="d5dae-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5dae-150">Here is a JSON representation of the resource.</span></span>

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