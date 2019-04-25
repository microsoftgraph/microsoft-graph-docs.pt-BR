---
title: tipo de recurso networkConnection
description: Contém informações de estado sobre a conexão de rede relacionada ao alerta.
localization_priority: Normal
ms.openlocfilehash: 78ddcfd19d68b8dcd64c74a5beed6d1430f0ca38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580272"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="00ff6-103">tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="00ff6-103">networkConnection resource type</span></span>

<span data-ttu-id="00ff6-104">Contém informações de estado sobre a conexão de rede relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="00ff6-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="00ff6-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00ff6-105">Properties</span></span>

| <span data-ttu-id="00ff6-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00ff6-106">Property</span></span>   | <span data-ttu-id="00ff6-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="00ff6-107">Type</span></span>|<span data-ttu-id="00ff6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="00ff6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00ff6-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="00ff6-109">applicationName</span></span>|<span data-ttu-id="00ff6-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="00ff6-110">String</span></span>|<span data-ttu-id="00ff6-111">Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP, etc.).</span><span class="sxs-lookup"><span data-stu-id="00ff6-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="00ff6-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="00ff6-112">destinationAddress</span></span>|<span data-ttu-id="00ff6-113">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-113">String</span></span>|<span data-ttu-id="00ff6-114">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="00ff6-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="00ff6-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="00ff6-115">destinationDomain</span></span>|<span data-ttu-id="00ff6-116">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-116">String</span></span>|<span data-ttu-id="00ff6-117">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="00ff6-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="00ff6-118">(por exemplo, ' www.contoso.com ').</span><span class="sxs-lookup"><span data-stu-id="00ff6-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="00ff6-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="00ff6-119">destinationPort</span></span>|<span data-ttu-id="00ff6-120">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-120">String</span></span>|<span data-ttu-id="00ff6-121">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="00ff6-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="00ff6-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="00ff6-122">destinationUrl</span></span>|<span data-ttu-id="00ff6-123">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-123">String</span></span>|<span data-ttu-id="00ff6-124">URL de conexão de rede/cadeia de caracteres URI-excluindo parâmetros.</span><span class="sxs-lookup"><span data-stu-id="00ff6-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="00ff6-125">(por exemplo, ' www.contoso.com/products/default.html ')</span><span class="sxs-lookup"><span data-stu-id="00ff6-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="00ff6-126">direction</span><span class="sxs-lookup"><span data-stu-id="00ff6-126">direction</span></span>|<span data-ttu-id="00ff6-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="00ff6-127">connectionDirection</span></span>|<span data-ttu-id="00ff6-128">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-128">Network connection direction.</span></span> <span data-ttu-id="00ff6-129">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="00ff6-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="00ff6-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="00ff6-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="00ff6-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00ff6-131">DateTimeOffset</span></span>|<span data-ttu-id="00ff6-132">Data em que o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="00ff6-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="00ff6-133">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="00ff6-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="00ff6-134">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="00ff6-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="00ff6-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="00ff6-135">localDnsName</span></span>|<span data-ttu-id="00ff6-136">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-136">String</span></span>|<span data-ttu-id="00ff6-137">A resolução de nome DNS local da forma como aparece no cache de DNS local do host (por exemplo, caso o arquivo "hosts" tenha sido adulterado).</span><span class="sxs-lookup"><span data-stu-id="00ff6-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="00ff6-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="00ff6-138">natDestinationAddress</span></span>|<span data-ttu-id="00ff6-139">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-139">String</span></span>|<span data-ttu-id="00ff6-140">Endereço IP de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="00ff6-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="00ff6-141">natDestinationPort</span></span>|<span data-ttu-id="00ff6-142">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-142">String</span></span>|<span data-ttu-id="00ff6-143">Porta de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="00ff6-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="00ff6-144">natSourceAddress</span></span>|<span data-ttu-id="00ff6-145">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-145">String</span></span>|<span data-ttu-id="00ff6-146">Endereço IP de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="00ff6-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="00ff6-147">natSourcePort</span></span>|<span data-ttu-id="00ff6-148">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-148">String</span></span>|<span data-ttu-id="00ff6-149">Porta de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="00ff6-150">RDP</span><span class="sxs-lookup"><span data-stu-id="00ff6-150">protocol</span></span>|[<span data-ttu-id="00ff6-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="00ff6-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="00ff6-152">Protocolo de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-152">Network protocol.</span></span> <span data-ttu-id="00ff6-153">Os valores possíveis são `unknown`: `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp` `ipv6` `ipv6RoutingHeader`,,, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` ,,,,,,,, , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="00ff6-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="00ff6-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="00ff6-154">riskScore</span></span>|<span data-ttu-id="00ff6-155">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-155">String</span></span>|<span data-ttu-id="00ff6-156">Provedor gerado/Pontuação de risco calculado da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="00ff6-157">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="00ff6-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="00ff6-158">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="00ff6-158">sourceAddress</span></span>|<span data-ttu-id="00ff6-159">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-159">String</span></span>|<span data-ttu-id="00ff6-160">Endereço IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="00ff6-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="00ff6-161">sourcePort</span><span class="sxs-lookup"><span data-stu-id="00ff6-161">sourcePort</span></span>|<span data-ttu-id="00ff6-162">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-162">String</span></span>|<span data-ttu-id="00ff6-163">Porta IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="00ff6-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="00ff6-164">status</span><span class="sxs-lookup"><span data-stu-id="00ff6-164">status</span></span>|<span data-ttu-id="00ff6-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="00ff6-165">connectionStatus</span></span>|<span data-ttu-id="00ff6-166">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="00ff6-166">Network connection status.</span></span> <span data-ttu-id="00ff6-167">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="00ff6-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="00ff6-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="00ff6-168">urlParameters</span></span>|<span data-ttu-id="00ff6-169">String</span><span class="sxs-lookup"><span data-stu-id="00ff6-169">String</span></span>|<span data-ttu-id="00ff6-170">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="00ff6-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00ff6-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00ff6-171">JSON representation</span></span>

<span data-ttu-id="00ff6-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00ff6-172">The following is a JSON representation of the resource.</span></span>

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
