# <a name="networkconnection-resource-type"></a><span data-ttu-id="033f1-101">tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="033f1-101">networkConnection resource type</span></span>

<span data-ttu-id="033f1-102">Contém informações com estado sobre a conexão de rede relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="033f1-102">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="033f1-103">Propriedades</span><span class="sxs-lookup"><span data-stu-id="033f1-103">Properties</span></span>

| <span data-ttu-id="033f1-104">Propriedade</span><span class="sxs-lookup"><span data-stu-id="033f1-104">Property</span></span>   | <span data-ttu-id="033f1-105">Tipo</span><span class="sxs-lookup"><span data-stu-id="033f1-105">Type</span></span>|<span data-ttu-id="033f1-106">Descrição</span><span class="sxs-lookup"><span data-stu-id="033f1-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="033f1-107">applicationName</span><span class="sxs-lookup"><span data-stu-id="033f1-107">applicationName</span></span>|<span data-ttu-id="033f1-108">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-108">String</span></span>|<span data-ttu-id="033f1-109">Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP, etc.).</span><span class="sxs-lookup"><span data-stu-id="033f1-109">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="033f1-110">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="033f1-110">destinationAddress</span></span>|<span data-ttu-id="033f1-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-111">String</span></span>|<span data-ttu-id="033f1-112">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="033f1-112">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="033f1-113">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="033f1-113">destinationDomain</span></span>|<span data-ttu-id="033f1-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-114">String</span></span>|<span data-ttu-id="033f1-115">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="033f1-115">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="033f1-116">(por exemplo 'www.contoso.com').</span><span class="sxs-lookup"><span data-stu-id="033f1-116">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="033f1-117">destinationPort</span><span class="sxs-lookup"><span data-stu-id="033f1-117">destinationPort</span></span>|<span data-ttu-id="033f1-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-118">String</span></span>|<span data-ttu-id="033f1-119">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="033f1-119">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="033f1-120">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="033f1-120">destinationUrl</span></span>|<span data-ttu-id="033f1-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-121">String</span></span>|<span data-ttu-id="033f1-122">Cadeia de caracteres de URL/URI de conexão de rede - excluindo parâmetros.</span><span class="sxs-lookup"><span data-stu-id="033f1-122">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="033f1-123">(por exemplo, 'www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="033f1-123">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="033f1-124">direção</span><span class="sxs-lookup"><span data-stu-id="033f1-124">direction</span></span>|<span data-ttu-id="033f1-125">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="033f1-125">connectionDirection</span></span>|<span data-ttu-id="033f1-126">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-126">Network connection direction.</span></span> <span data-ttu-id="033f1-127">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="033f1-127">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="033f1-128">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="033f1-128">domainRegisteredDateTime</span></span>|<span data-ttu-id="033f1-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="033f1-129">DateTimeOffset</span></span>|<span data-ttu-id="033f1-130">Data quando o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="033f1-130">Date when the destination domain was registered.</span></span> <span data-ttu-id="033f1-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="033f1-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="033f1-132">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="033f1-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="033f1-133">localDnsName</span><span class="sxs-lookup"><span data-stu-id="033f1-133">localDnsName</span></span>|<span data-ttu-id="033f1-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-134">String</span></span>|<span data-ttu-id="033f1-135">A resolução do nome DNS local como aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' tenha sido adulterado).</span><span class="sxs-lookup"><span data-stu-id="033f1-135">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="033f1-136">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="033f1-136">natDestinationAddress</span></span>|<span data-ttu-id="033f1-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-137">String</span></span>|<span data-ttu-id="033f1-138">Endereço IP de destino da Conversão de Endereços de Rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-138">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="033f1-139">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="033f1-139">natDestinationPort</span></span>|<span data-ttu-id="033f1-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-140">String</span></span>|<span data-ttu-id="033f1-141">Porta de destino de Conversão de Endereços de Rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-141">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="033f1-142">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="033f1-142">natSourceAddress</span></span>|<span data-ttu-id="033f1-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-143">String</span></span>|<span data-ttu-id="033f1-144">Endereço IP de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-144">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="033f1-145">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="033f1-145">natSourcePort</span></span>|<span data-ttu-id="033f1-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-146">String</span></span>|<span data-ttu-id="033f1-147">Porta de origem da Conversão de Endereços de Rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-147">Network Address Translation source port.</span></span>|
|<span data-ttu-id="033f1-148">protocolo</span><span class="sxs-lookup"><span data-stu-id="033f1-148">protocol</span></span>|[<span data-ttu-id="033f1-149">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="033f1-149">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="033f1-150">Protocolo de Rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-150">Network protocol analysis</span></span> <span data-ttu-id="033f1-151">Os valores possíveis são: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="033f1-151">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`.</span></span>|
|<span data-ttu-id="033f1-152">riskScore</span><span class="sxs-lookup"><span data-stu-id="033f1-152">riskScore</span></span>|<span data-ttu-id="033f1-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-153">String</span></span>|<span data-ttu-id="033f1-154">Pontuação de risco gerada/calculada pelo provedor da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-154">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="033f1-155">Intervalo de valor recomendado de 0-1, que equivale a um percentual.</span><span class="sxs-lookup"><span data-stu-id="033f1-155">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="033f1-156">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="033f1-156">sourceAddress</span></span>|<span data-ttu-id="033f1-157">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-157">String</span></span>|<span data-ttu-id="033f1-158">Endereço IP de origem (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="033f1-158">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="033f1-159">sourcePort</span><span class="sxs-lookup"><span data-stu-id="033f1-159">sourcePort</span></span>|<span data-ttu-id="033f1-160">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-160">String</span></span>|<span data-ttu-id="033f1-161">Porta do IP de origem (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="033f1-161">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="033f1-162">status</span><span class="sxs-lookup"><span data-stu-id="033f1-162">status</span></span>|<span data-ttu-id="033f1-163">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="033f1-163">ConnectionStatus</span></span>|<span data-ttu-id="033f1-164">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="033f1-164">Network connection status.</span></span> <span data-ttu-id="033f1-165">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="033f1-165">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="033f1-166">urlParameters</span><span class="sxs-lookup"><span data-stu-id="033f1-166">urlParameters</span></span>|<span data-ttu-id="033f1-167">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="033f1-167">String</span></span>|<span data-ttu-id="033f1-168">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="033f1-168">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="033f1-169">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="033f1-169">JSON representation</span></span>

<span data-ttu-id="033f1-170">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="033f1-170">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.networkConnection"
}-->

```json
{
  "applicationName": "String",
  "destinationAddress": "String",
  "destinationDomain": "String",
  "destinationPort": "String",
  "destinationUrl": "String",
  "direction": "@odata.type: microsoft.graph.connectionDirection",
  "domainRegisteredDateTime": "String (timestamp)",
  "localDnsName": "String",
  "natDestinationAddress": "String",
  "natDestinationPort": "String",
  "natSourceAddress": "String",
  "natSourcePort": "String",
  "protocol": "@odata.type: microsoft.graph.securityNetworkProtocol",
  "riskScore": "String",
  "sourceAddress": "String",
  "sourcePort": "String",
  "status": "@odata.type: microsoft.graph.connectionStatus",
  "urlParameters": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->