---
title: tipo de recurso networkConnection
description: Contém informações de estado sobre a conexão de rede relacionada ao alerta.
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 72fcfcd3c6849e9c8e9f05b50671e1aa611dc129
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44682051"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="791e1-103">tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="791e1-103">networkConnection resource type</span></span>

<span data-ttu-id="791e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="791e1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="791e1-105">Contém informações de estado sobre a conexão de rede relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="791e1-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="791e1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="791e1-106">Properties</span></span>

| <span data-ttu-id="791e1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="791e1-107">Property</span></span>   | <span data-ttu-id="791e1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="791e1-108">Type</span></span>|<span data-ttu-id="791e1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="791e1-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="791e1-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="791e1-110">applicationName</span></span>|<span data-ttu-id="791e1-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="791e1-111">String</span></span>|<span data-ttu-id="791e1-112">Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook ou SMTP).</span><span class="sxs-lookup"><span data-stu-id="791e1-112">Name of the application managing the network connection (for example, Facebook or SMTP).</span></span>|
|<span data-ttu-id="791e1-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="791e1-113">destinationAddress</span></span>|<span data-ttu-id="791e1-114">String</span><span class="sxs-lookup"><span data-stu-id="791e1-114">String</span></span>|<span data-ttu-id="791e1-115">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="791e1-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="791e1-116">destinationLocation</span><span class="sxs-lookup"><span data-stu-id="791e1-116">destinationLocation</span></span>|<span data-ttu-id="791e1-117">String</span><span class="sxs-lookup"><span data-stu-id="791e1-117">String</span></span>|<span data-ttu-id="791e1-118">Local (por mapeamento de endereço IP) associado ao destino de uma conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-118">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="791e1-119">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="791e1-119">destinationDomain</span></span>|<span data-ttu-id="791e1-120">String</span><span class="sxs-lookup"><span data-stu-id="791e1-120">String</span></span>|<span data-ttu-id="791e1-121">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="791e1-121">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="791e1-122">(por exemplo, ' www.contoso.com ').</span><span class="sxs-lookup"><span data-stu-id="791e1-122">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="791e1-123">destinationPort</span><span class="sxs-lookup"><span data-stu-id="791e1-123">destinationPort</span></span>|<span data-ttu-id="791e1-124">String</span><span class="sxs-lookup"><span data-stu-id="791e1-124">String</span></span>|<span data-ttu-id="791e1-125">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="791e1-125">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="791e1-126">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="791e1-126">destinationUrl</span></span>|<span data-ttu-id="791e1-127">String</span><span class="sxs-lookup"><span data-stu-id="791e1-127">String</span></span>|<span data-ttu-id="791e1-128">URL de conexão de rede/cadeia de caracteres URI-excluindo parâmetros.</span><span class="sxs-lookup"><span data-stu-id="791e1-128">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="791e1-129">(por exemplo, ' www.contoso.com/products/default.htmL')</span><span class="sxs-lookup"><span data-stu-id="791e1-129">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="791e1-130">direction</span><span class="sxs-lookup"><span data-stu-id="791e1-130">direction</span></span>|<span data-ttu-id="791e1-131">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="791e1-131">connectionDirection</span></span>|<span data-ttu-id="791e1-132">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-132">Network connection direction.</span></span> <span data-ttu-id="791e1-133">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="791e1-133">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="791e1-134">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="791e1-134">domainRegisteredDateTime</span></span>|<span data-ttu-id="791e1-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="791e1-135">DateTimeOffset</span></span>|<span data-ttu-id="791e1-136">Data em que o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="791e1-136">Date when the destination domain was registered.</span></span> <span data-ttu-id="791e1-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="791e1-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="791e1-138">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="791e1-138">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="791e1-139">localDnsName</span><span class="sxs-lookup"><span data-stu-id="791e1-139">localDnsName</span></span>|<span data-ttu-id="791e1-140">String</span><span class="sxs-lookup"><span data-stu-id="791e1-140">String</span></span>|<span data-ttu-id="791e1-141">A resolução de nome DNS local da forma como aparece no cache de DNS local do host (por exemplo, caso o arquivo "hosts" tenha sido adulterado).</span><span class="sxs-lookup"><span data-stu-id="791e1-141">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="791e1-142">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="791e1-142">natDestinationAddress</span></span>|<span data-ttu-id="791e1-143">String</span><span class="sxs-lookup"><span data-stu-id="791e1-143">String</span></span>|<span data-ttu-id="791e1-144">Endereço IP de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-144">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="791e1-145">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="791e1-145">natDestinationPort</span></span>|<span data-ttu-id="791e1-146">String</span><span class="sxs-lookup"><span data-stu-id="791e1-146">String</span></span>|<span data-ttu-id="791e1-147">Porta de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-147">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="791e1-148">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="791e1-148">natSourceAddress</span></span>|<span data-ttu-id="791e1-149">String</span><span class="sxs-lookup"><span data-stu-id="791e1-149">String</span></span>|<span data-ttu-id="791e1-150">Endereço IP de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-150">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="791e1-151">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="791e1-151">natSourcePort</span></span>|<span data-ttu-id="791e1-152">String</span><span class="sxs-lookup"><span data-stu-id="791e1-152">String</span></span>|<span data-ttu-id="791e1-153">Porta de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-153">Network Address Translation source port.</span></span>|
|<span data-ttu-id="791e1-154">RDP</span><span class="sxs-lookup"><span data-stu-id="791e1-154">protocol</span></span>|[<span data-ttu-id="791e1-155">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="791e1-155">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="791e1-156">Protocolo de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-156">Network protocol.</span></span> <span data-ttu-id="791e1-157">Os valores possíveis são:,,,,,,,,,,,,,,,,,,,, `unknown` `ip` `icmp` `igmp` `ggp` `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` , `ipSecEncapsulatingSecurityPayload` , `ipSecAuthenticationHeader` ,, `icmpV6` `ipv6NoNextHeader` , `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII` ,,,,,.</span><span class="sxs-lookup"><span data-stu-id="791e1-157">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="791e1-158">riskScore</span><span class="sxs-lookup"><span data-stu-id="791e1-158">riskScore</span></span>|<span data-ttu-id="791e1-159">String</span><span class="sxs-lookup"><span data-stu-id="791e1-159">String</span></span>|<span data-ttu-id="791e1-160">Provedor gerado/Pontuação de risco calculado da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-160">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="791e1-161">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="791e1-161">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="791e1-162">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="791e1-162">sourceAddress</span></span>|<span data-ttu-id="791e1-163">String</span><span class="sxs-lookup"><span data-stu-id="791e1-163">String</span></span>|<span data-ttu-id="791e1-164">Endereço IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="791e1-164">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="791e1-165">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="791e1-165">sourceLocation</span></span>|<span data-ttu-id="791e1-166">String</span><span class="sxs-lookup"><span data-stu-id="791e1-166">String</span></span>|<span data-ttu-id="791e1-167">Local (por mapeamento de endereço IP) associado à origem de uma conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-167">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="791e1-168">sourcePort</span><span class="sxs-lookup"><span data-stu-id="791e1-168">sourcePort</span></span>|<span data-ttu-id="791e1-169">String</span><span class="sxs-lookup"><span data-stu-id="791e1-169">String</span></span>|<span data-ttu-id="791e1-170">Porta IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="791e1-170">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="791e1-171">status</span><span class="sxs-lookup"><span data-stu-id="791e1-171">status</span></span>|<span data-ttu-id="791e1-172">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="791e1-172">connectionStatus</span></span>|<span data-ttu-id="791e1-173">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="791e1-173">Network connection status.</span></span> <span data-ttu-id="791e1-174">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="791e1-174">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="791e1-175">urlParameters</span><span class="sxs-lookup"><span data-stu-id="791e1-175">urlParameters</span></span>|<span data-ttu-id="791e1-176">String</span><span class="sxs-lookup"><span data-stu-id="791e1-176">String</span></span>|<span data-ttu-id="791e1-177">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="791e1-177">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="791e1-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="791e1-178">JSON representation</span></span>

<span data-ttu-id="791e1-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="791e1-179">The following is a JSON representation of the resource.</span></span>

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
  "destinationLocation": "String",
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
  "sourceLocation": "String",
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
