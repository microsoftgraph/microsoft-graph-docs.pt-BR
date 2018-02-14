# <a name="proxieddomain-resource-type"></a><span data-ttu-id="836dd-101">Tipo de recurso proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="836dd-101">proxiedDomain resource type</span></span>

> <span data-ttu-id="836dd-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="836dd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="836dd-103">Domínio com proxy</span><span class="sxs-lookup"><span data-stu-id="836dd-103">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="836dd-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="836dd-104">Properties</span></span>
|<span data-ttu-id="836dd-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="836dd-105">Property</span></span>|<span data-ttu-id="836dd-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="836dd-106">Type</span></span>|<span data-ttu-id="836dd-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="836dd-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="836dd-108">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="836dd-108">ipAddressOrFQDN</span></span>|<span data-ttu-id="836dd-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="836dd-109">String</span></span>|<span data-ttu-id="836dd-110">O endereço IP ou FQDN</span><span class="sxs-lookup"><span data-stu-id="836dd-110">The IP address or FQDN</span></span>|
|<span data-ttu-id="836dd-111">proxy</span><span class="sxs-lookup"><span data-stu-id="836dd-111">web proxy</span></span>|<span data-ttu-id="836dd-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="836dd-112">String</span></span>|<span data-ttu-id="836dd-113">IP de proxy</span><span class="sxs-lookup"><span data-stu-id="836dd-113">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="836dd-114">Relações</span><span class="sxs-lookup"><span data-stu-id="836dd-114">Relationships</span></span>
<span data-ttu-id="836dd-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="836dd-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="836dd-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="836dd-116">JSON Representation</span></span>
<span data-ttu-id="836dd-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="836dd-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```



