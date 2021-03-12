---
title: Tipo de recurso networkConnection
description: Contém informações de estado sobre a conexão de rede relacionada ao alerta.
localization_priority: Normal
author: chinguyen1
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 5671726ead3da811c109a9a2afe01c49b665e513
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719007"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="8364f-103">Tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="8364f-103">networkConnection resource type</span></span>

<span data-ttu-id="8364f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8364f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8364f-105">Contém informações de estado sobre a conexão de rede relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="8364f-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="8364f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8364f-106">Properties</span></span>

| <span data-ttu-id="8364f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8364f-107">Property</span></span>   | <span data-ttu-id="8364f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8364f-108">Type</span></span>|<span data-ttu-id="8364f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8364f-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8364f-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="8364f-110">applicationName</span></span>|<span data-ttu-id="8364f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-111">String</span></span>|<span data-ttu-id="8364f-112">Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook ou SMTP).</span><span class="sxs-lookup"><span data-stu-id="8364f-112">Name of the application managing the network connection (for example, Facebook or SMTP).</span></span>|
|<span data-ttu-id="8364f-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="8364f-113">destinationAddress</span></span>|<span data-ttu-id="8364f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-114">String</span></span>|<span data-ttu-id="8364f-115">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="8364f-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="8364f-116">destinationLocation</span><span class="sxs-lookup"><span data-stu-id="8364f-116">destinationLocation</span></span>|<span data-ttu-id="8364f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-117">String</span></span>|<span data-ttu-id="8364f-118">Local (por mapeamento de endereço IP) associado ao destino de uma conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-118">Location (by IP address mapping) associated with the destination of a network connection.</span></span>|
|<span data-ttu-id="8364f-119">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="8364f-119">destinationDomain</span></span>|<span data-ttu-id="8364f-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-120">String</span></span>|<span data-ttu-id="8364f-121">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="8364f-121">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="8364f-122">(por exemplo, 'www.contoso.com').</span><span class="sxs-lookup"><span data-stu-id="8364f-122">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="8364f-123">destinationPort</span><span class="sxs-lookup"><span data-stu-id="8364f-123">destinationPort</span></span>|<span data-ttu-id="8364f-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-124">String</span></span>|<span data-ttu-id="8364f-125">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="8364f-125">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="8364f-126">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="8364f-126">destinationUrl</span></span>|<span data-ttu-id="8364f-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-127">String</span></span>|<span data-ttu-id="8364f-128">Cadeia de caracteres url/URI de conexão de rede - excluindo parâmetros.</span><span class="sxs-lookup"><span data-stu-id="8364f-128">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="8364f-129">(por exemplo, 'www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="8364f-129">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="8364f-130">direction</span><span class="sxs-lookup"><span data-stu-id="8364f-130">direction</span></span>|<span data-ttu-id="8364f-131">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="8364f-131">connectionDirection</span></span>|<span data-ttu-id="8364f-132">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-132">Network connection direction.</span></span> <span data-ttu-id="8364f-133">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="8364f-133">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="8364f-134">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="8364f-134">domainRegisteredDateTime</span></span>|<span data-ttu-id="8364f-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8364f-135">DateTimeOffset</span></span>|<span data-ttu-id="8364f-136">Data em que o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="8364f-136">Date when the destination domain was registered.</span></span> <span data-ttu-id="8364f-137">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="8364f-137">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="8364f-138">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="8364f-138">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="8364f-139">localDnsName</span><span class="sxs-lookup"><span data-stu-id="8364f-139">localDnsName</span></span>|<span data-ttu-id="8364f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-140">String</span></span>|<span data-ttu-id="8364f-141">A resolução de nome DNS local como ela aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' tenha sido adulterado).</span><span class="sxs-lookup"><span data-stu-id="8364f-141">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="8364f-142">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="8364f-142">natDestinationAddress</span></span>|<span data-ttu-id="8364f-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-143">String</span></span>|<span data-ttu-id="8364f-144">Endereço de rede Endereço endereço endereço IP de destino.</span><span class="sxs-lookup"><span data-stu-id="8364f-144">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="8364f-145">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="8364f-145">natDestinationPort</span></span>|<span data-ttu-id="8364f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-146">String</span></span>|<span data-ttu-id="8364f-147">Porta de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-147">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="8364f-148">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="8364f-148">natSourceAddress</span></span>|<span data-ttu-id="8364f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-149">String</span></span>|<span data-ttu-id="8364f-150">Endereço de rede Endereço endereço IP de origem.</span><span class="sxs-lookup"><span data-stu-id="8364f-150">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="8364f-151">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="8364f-151">natSourcePort</span></span>|<span data-ttu-id="8364f-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-152">String</span></span>|<span data-ttu-id="8364f-153">Porta de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-153">Network Address Translation source port.</span></span>|
|<span data-ttu-id="8364f-154">protocol</span><span class="sxs-lookup"><span data-stu-id="8364f-154">protocol</span></span>|[<span data-ttu-id="8364f-155">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="8364f-155">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="8364f-156">Protocolo de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-156">Network protocol.</span></span> <span data-ttu-id="8364f-157">Os valores possíveis são: `unknown` , , , , , , , , `ip` `icmp` , `igmp` `ggp` , `ipv4` `tcp` `pup` `udp` `idp` `ipv6` `ipv6RoutingHeader` `ipv6FragmentHeader` `ipSecEncapsulatingSecurityPayload` `ipSecAuthenticationHeader` , `icmpV6` `ipv6NoNextHeader` `ipv6DestinationOptions` `nd` `raw` `ipx` `spx` `spxII`</span><span class="sxs-lookup"><span data-stu-id="8364f-157">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="8364f-158">riskScore</span><span class="sxs-lookup"><span data-stu-id="8364f-158">riskScore</span></span>|<span data-ttu-id="8364f-159">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-159">String</span></span>|<span data-ttu-id="8364f-160">Pontuação de risco gerada/calculada do provedor da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-160">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="8364f-161">Intervalo de valores recomendado de 0 a 1, que equivale a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="8364f-161">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="8364f-162">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="8364f-162">sourceAddress</span></span>|<span data-ttu-id="8364f-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-163">String</span></span>|<span data-ttu-id="8364f-164">Endereço IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="8364f-164">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="8364f-165">sourceLocation</span><span class="sxs-lookup"><span data-stu-id="8364f-165">sourceLocation</span></span>|<span data-ttu-id="8364f-166">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-166">String</span></span>|<span data-ttu-id="8364f-167">Local (por mapeamento de endereço IP) associado à origem de uma conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-167">Location (by IP address mapping) associated with the source of a network connection.</span></span>|
|<span data-ttu-id="8364f-168">sourcePort</span><span class="sxs-lookup"><span data-stu-id="8364f-168">sourcePort</span></span>|<span data-ttu-id="8364f-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-169">String</span></span>|<span data-ttu-id="8364f-170">Porta IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="8364f-170">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="8364f-171">status</span><span class="sxs-lookup"><span data-stu-id="8364f-171">status</span></span>|<span data-ttu-id="8364f-172">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="8364f-172">connectionStatus</span></span>|<span data-ttu-id="8364f-173">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="8364f-173">Network connection status.</span></span> <span data-ttu-id="8364f-174">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="8364f-174">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="8364f-175">urlParameters</span><span class="sxs-lookup"><span data-stu-id="8364f-175">urlParameters</span></span>|<span data-ttu-id="8364f-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8364f-176">String</span></span>|<span data-ttu-id="8364f-177">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="8364f-177">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8364f-178">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8364f-178">JSON representation</span></span>

<span data-ttu-id="8364f-179">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8364f-179">The following is a JSON representation of the resource.</span></span>

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

