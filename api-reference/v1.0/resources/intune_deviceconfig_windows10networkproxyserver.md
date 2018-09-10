# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="daf90-101">Tipo de recurso windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="daf90-101">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="daf90-102">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="daf90-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="daf90-103">Política de Servidor Proxy de Rede.</span><span class="sxs-lookup"><span data-stu-id="daf90-103">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="daf90-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="daf90-104">Properties</span></span>
|<span data-ttu-id="daf90-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="daf90-105">Property</span></span>|<span data-ttu-id="daf90-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="daf90-106">Type</span></span>|<span data-ttu-id="daf90-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="daf90-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf90-108">address</span><span class="sxs-lookup"><span data-stu-id="daf90-108">address</span></span>|<span data-ttu-id="daf90-109">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="daf90-109">String</span></span>|<span data-ttu-id="daf90-110">Endereço para o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="daf90-110">Address to the proxy server.</span></span> <span data-ttu-id="daf90-111">Especifique um endereço no formato <server>\[“:”<port>\]</span><span class="sxs-lookup"><span data-stu-id="daf90-111">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="daf90-112">exceptions</span><span class="sxs-lookup"><span data-stu-id="daf90-112">exceptions</span></span>|<span data-ttu-id="daf90-113">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="daf90-113">String collection</span></span>|<span data-ttu-id="daf90-114">Endereços que não devem usar o servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="daf90-114">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="daf90-115">O sistema não usará o servidor proxy para endereços que começam com o conteúdo especificado nesse nó.</span><span class="sxs-lookup"><span data-stu-id="daf90-115">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="daf90-116">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="daf90-116">useForLocalAddresses</span></span>|<span data-ttu-id="daf90-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="daf90-117">Boolean</span></span>|<span data-ttu-id="daf90-118">Especifica se o servidor proxy deve ser usado para endereços locais (intranet).</span><span class="sxs-lookup"><span data-stu-id="daf90-118">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="daf90-119">Relações</span><span class="sxs-lookup"><span data-stu-id="daf90-119">Relationships</span></span>
<span data-ttu-id="daf90-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="daf90-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="daf90-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="daf90-121">JSON Representation</span></span>
<span data-ttu-id="daf90-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="daf90-122">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```








