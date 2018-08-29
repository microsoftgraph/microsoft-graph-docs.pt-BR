# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="b6757-101">Tipo de recurso windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="b6757-101">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="b6757-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6757-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6757-103">Coleção de domínios como proxy da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="b6757-103">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="b6757-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6757-104">Properties</span></span>
|<span data-ttu-id="b6757-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6757-105">Property</span></span>|<span data-ttu-id="b6757-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6757-106">Type</span></span>|<span data-ttu-id="b6757-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6757-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6757-108">displayName</span><span class="sxs-lookup"><span data-stu-id="b6757-108">displayName</span></span>|<span data-ttu-id="b6757-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b6757-109">String</span></span>|<span data-ttu-id="b6757-110">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="b6757-110">Display name</span></span>|
|<span data-ttu-id="b6757-111">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="b6757-111">proxiedDomains</span></span>|<span data-ttu-id="b6757-112">Coleção [proxiedDomain](../resources/intune_mam_proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="b6757-112">[proxiedDomain](../resources/intune_mam_proxieddomain.md) collection</span></span>|<span data-ttu-id="b6757-113">Coleção de domínios com proxy</span><span class="sxs-lookup"><span data-stu-id="b6757-113">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6757-114">Relações</span><span class="sxs-lookup"><span data-stu-id="b6757-114">Relationships</span></span>
<span data-ttu-id="b6757-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6757-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b6757-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6757-116">JSON Representation</span></span>
<span data-ttu-id="b6757-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6757-117">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```



