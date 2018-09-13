# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="d953b-101">tipo de recurso cloudAppSecurityState</span><span class="sxs-lookup"><span data-stu-id="d953b-101">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="d953b-102">Contém informações com estado sobre o aplicativo na nuvem (destinationServiceName, destinationServiceIp).</span><span class="sxs-lookup"><span data-stu-id="d953b-102">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="d953b-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d953b-103">Properties</span></span>

| <span data-ttu-id="d953b-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d953b-104">Property</span></span>     | <span data-ttu-id="d953b-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="d953b-105">Type</span></span>        | <span data-ttu-id="d953b-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="d953b-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d953b-107">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="d953b-107">destinationServiceIp</span></span>|<span data-ttu-id="d953b-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d953b-108">String</span></span>|<span data-ttu-id="d953b-109">Endereço IP de destino da conexão para o serviço/aplicativo em nuvem.</span><span class="sxs-lookup"><span data-stu-id="d953b-109">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="d953b-110">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="d953b-110">destinationServiceName</span></span>|<span data-ttu-id="d953b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d953b-111">String</span></span>|<span data-ttu-id="d953b-112">Nome do serviço do aplicativo na nuvem (por exemplo "Equipe de vendas", "Recados", etc.).</span><span class="sxs-lookup"><span data-stu-id="d953b-112">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="d953b-113">riskScore</span><span class="sxs-lookup"><span data-stu-id="d953b-113">riskScore</span></span>|<span data-ttu-id="d953b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d953b-114">String</span></span>|<span data-ttu-id="d953b-115">Pontuação de risco calculada/gerada pelo provedor do aplicativo/serviço na nuvem.</span><span class="sxs-lookup"><span data-stu-id="d953b-115">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="d953b-116">Intervalo de valor recomendado de 0-1, que equivale a um percentual.</span><span class="sxs-lookup"><span data-stu-id="d953b-116">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d953b-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d953b-117">JSON representation</span></span>

<span data-ttu-id="d953b-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d953b-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->