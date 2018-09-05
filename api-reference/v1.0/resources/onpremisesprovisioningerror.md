# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="b04fa-101">tipo de recurso onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="b04fa-101">onPremisesProvisioningError resource type</span></span>

<span data-ttu-id="b04fa-102">Representa os erros de sincronização de diretório para as entidades de [usuário](user.md) e [grupo](group.md) quando durante a sincronização local de diretórios no Active Directory do Azure.</span><span class="sxs-lookup"><span data-stu-id="b04fa-102">Represents directory synchronization errors for the [user](user.md) and [group](group.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="b04fa-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b04fa-103">Properties</span></span>

| <span data-ttu-id="b04fa-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b04fa-104">Property</span></span> | <span data-ttu-id="b04fa-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="b04fa-105">Type</span></span> | <span data-ttu-id="b04fa-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="b04fa-106">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="b04fa-107">category</span><span class="sxs-lookup"><span data-stu-id="b04fa-107">category</span></span>|<span data-ttu-id="b04fa-108">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b04fa-108">String</span></span>| <span data-ttu-id="b04fa-109">Categoria do erro de configuração.</span><span class="sxs-lookup"><span data-stu-id="b04fa-109">Category of the provisioning error.</span></span> <span data-ttu-id="b04fa-110">Observação: No momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="b04fa-110">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="b04fa-111">Valor possível: *PropertyConflict* - indica que o valor de uma propriedade não é único.</span><span class="sxs-lookup"><span data-stu-id="b04fa-111">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="b04fa-112">Outros objetos contêm o mesmo valor para a propriedade.</span><span class="sxs-lookup"><span data-stu-id="b04fa-112">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="b04fa-113">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="b04fa-113">occurredDateTime</span></span>|<span data-ttu-id="b04fa-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b04fa-114">DateTimeOffset</span></span>| <span data-ttu-id="b04fa-115">A data e hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="b04fa-115">The time at which the error occurred.</span></span> |
|<span data-ttu-id="b04fa-116">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="b04fa-116">propertyCausingError</span></span>|<span data-ttu-id="b04fa-117">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b04fa-117">String</span></span>| <span data-ttu-id="b04fa-118">Nome da propriedade de diretório que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="b04fa-118">Name of the directory property causing the error.</span></span> <span data-ttu-id="b04fa-119">Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="b04fa-119">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="b04fa-120">value</span><span class="sxs-lookup"><span data-stu-id="b04fa-120">value</span></span>|<span data-ttu-id="b04fa-121">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="b04fa-121">String</span></span>| <span data-ttu-id="b04fa-122">Valor da propriedade que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="b04fa-122">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b04fa-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b04fa-123">JSON representation</span></span>
<span data-ttu-id="b04fa-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b04fa-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->