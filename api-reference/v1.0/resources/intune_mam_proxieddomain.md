# <a name="proxieddomain-resource-type"></a><span data-ttu-id="157f6-101">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="157f6-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="157f6-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="157f6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="157f6-103">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="157f6-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="157f6-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="157f6-104">Properties</span></span>
|<span data-ttu-id="157f6-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="157f6-105">Property</span></span>|<span data-ttu-id="157f6-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="157f6-106">Type</span></span>|<span data-ttu-id="157f6-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="157f6-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="157f6-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="157f6-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="157f6-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="157f6-109">String</span></span>|<span data-ttu-id="157f6-110">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="157f6-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="157f6-111">proxy</span><span class="sxs-lookup"><span data-stu-id="157f6-111">proxy</span></span>|<span data-ttu-id="157f6-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="157f6-112">String</span></span>|<span data-ttu-id="157f6-113">IP de proxy</span><span class="sxs-lookup"><span data-stu-id="157f6-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="157f6-114">Relações</span><span class="sxs-lookup"><span data-stu-id="157f6-114">Relationships</span></span>
<span data-ttu-id="157f6-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="157f6-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="157f6-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="157f6-116">JSON Representation</span></span>
<span data-ttu-id="157f6-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="157f6-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```








