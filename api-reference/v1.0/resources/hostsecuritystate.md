# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="8eebe-101">tipo de recurso hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="8eebe-101">hostSecurityState resource type</span></span>

<span data-ttu-id="8eebe-102">Contém informações com estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="8eebe-102">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="8eebe-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8eebe-103">Properties</span></span>

| <span data-ttu-id="8eebe-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eebe-104">Property</span></span>   | <span data-ttu-id="8eebe-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eebe-105">Type</span></span>|<span data-ttu-id="8eebe-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eebe-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8eebe-107">fqdn</span><span class="sxs-lookup"><span data-stu-id="8eebe-107">FQDN</span></span>|<span data-ttu-id="8eebe-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eebe-108">String</span></span>|<span data-ttu-id="8eebe-109">FQDN do host (nome de domínio totalmente qualificado) (por exemplo, `machine.company.com`).</span><span class="sxs-lookup"><span data-stu-id="8eebe-109">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="8eebe-110">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="8eebe-110">isAzureAadJoined</span></span>|<span data-ttu-id="8eebe-111">Booleano</span><span class="sxs-lookup"><span data-stu-id="8eebe-111">Boolean</span></span>|<span data-ttu-id="8eebe-112">Verdadeiro se o host estiver associado aos serviços de domínio do Active Directory do Azure.</span><span class="sxs-lookup"><span data-stu-id="8eebe-112">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="8eebe-113">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="8eebe-113">isAzureAadRegistered</span></span>|<span data-ttu-id="8eebe-114">Booleano</span><span class="sxs-lookup"><span data-stu-id="8eebe-114">Boolean</span></span>|<span data-ttu-id="8eebe-115">Verdadeiro se o host estiver registrado no Registro de Dispositivos do Active Directory do Azure (dispositivos BYOD - ou seja, não totalmente gerenciados pela empresa).</span><span class="sxs-lookup"><span data-stu-id="8eebe-115">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="8eebe-116">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="8eebe-116">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="8eebe-117">Booleano</span><span class="sxs-lookup"><span data-stu-id="8eebe-117">Boolean</span></span>|<span data-ttu-id="8eebe-118">Verdadeiro se o host estiver associado a um domínio do Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="8eebe-118">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="8eebe-119">netBiosName</span><span class="sxs-lookup"><span data-stu-id="8eebe-119">netBiosName</span></span>|<span data-ttu-id="8eebe-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eebe-120">String</span></span>|<span data-ttu-id="8eebe-121">O nome do host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="8eebe-121">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="8eebe-122">os</span><span class="sxs-lookup"><span data-stu-id="8eebe-122">OS</span></span>|<span data-ttu-id="8eebe-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eebe-123">String</span></span>|<span data-ttu-id="8eebe-124">Sistema operacional do host.</span><span class="sxs-lookup"><span data-stu-id="8eebe-124">Host Operating System.</span></span> <span data-ttu-id="8eebe-125">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="8eebe-125">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="8eebe-126">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="8eebe-126">privateIpAddress</span></span>|<span data-ttu-id="8eebe-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eebe-127">String</span></span>|<span data-ttu-id="8eebe-128">Endereço particular IPv4 ou IPv6 (não roteável) (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="8eebe-128">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="8eebe-129">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="8eebe-129">publicIpAddress</span></span>|<span data-ttu-id="8eebe-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eebe-130">String</span></span>|<span data-ttu-id="8eebe-131">Endereço IPv4 ou IPv6 publicamente roteável (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="8eebe-131">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="8eebe-132">riskScore</span><span class="sxs-lookup"><span data-stu-id="8eebe-132">riskScore</span></span>|<span data-ttu-id="8eebe-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8eebe-133">String</span></span>|<span data-ttu-id="8eebe-134">Pontuação de risco do host gerada/calculada pelo provedor.</span><span class="sxs-lookup"><span data-stu-id="8eebe-134">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="8eebe-135">Intervalo de valor recomendado de 0-1, que equivale a um percentual.</span><span class="sxs-lookup"><span data-stu-id="8eebe-135">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8eebe-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8eebe-136">JSON representation</span></span>

<span data-ttu-id="8eebe-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8eebe-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
