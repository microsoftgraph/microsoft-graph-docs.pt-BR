---
title: tipo de recurso networkConnection
description: Contém informações com informações de estado sobre a conexão de rede relacionado ao alerta.
ms.openlocfilehash: e3352cbda430412691285c209c566fb379045681
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007122"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="dc52d-103">tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="dc52d-103">networkConnection resource type</span></span>

<span data-ttu-id="dc52d-104">Contém informações com informações de estado sobre a conexão de rede relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="dc52d-104">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="dc52d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dc52d-105">Properties</span></span>

| <span data-ttu-id="dc52d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dc52d-106">Property</span></span>   | <span data-ttu-id="dc52d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="dc52d-107">Type</span></span>|<span data-ttu-id="dc52d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="dc52d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc52d-109">applicationName</span><span class="sxs-lookup"><span data-stu-id="dc52d-109">applicationName</span></span>|<span data-ttu-id="dc52d-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dc52d-110">String</span></span>|<span data-ttu-id="dc52d-111">Nome do aplicativo de gerenciamento de conexão de rede (por exemplo, Facebook, SMTP, etc.).</span><span class="sxs-lookup"><span data-stu-id="dc52d-111">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="dc52d-112">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="dc52d-112">destinationAddress</span></span>|<span data-ttu-id="dc52d-113">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-113">String</span></span>|<span data-ttu-id="dc52d-114">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="dc52d-114">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="dc52d-115">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="dc52d-115">destinationDomain</span></span>|<span data-ttu-id="dc52d-116">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-116">String</span></span>|<span data-ttu-id="dc52d-117">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="dc52d-117">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="dc52d-118">(por exemplo 'www.contoso.com').</span><span class="sxs-lookup"><span data-stu-id="dc52d-118">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="dc52d-119">destinationPort</span><span class="sxs-lookup"><span data-stu-id="dc52d-119">destinationPort</span></span>|<span data-ttu-id="dc52d-120">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-120">String</span></span>|<span data-ttu-id="dc52d-121">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="dc52d-121">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="dc52d-122">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="dc52d-122">destinationUrl</span></span>|<span data-ttu-id="dc52d-123">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-123">String</span></span>|<span data-ttu-id="dc52d-124">Cadeia de caracteres de URL/URI de conexão - excluindo os parâmetros de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-124">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="dc52d-125">(por exemplo, 'www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="dc52d-125">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="dc52d-126">direção</span><span class="sxs-lookup"><span data-stu-id="dc52d-126">direction</span></span>|<span data-ttu-id="dc52d-127">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="dc52d-127">connectionDirection</span></span>|<span data-ttu-id="dc52d-128">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-128">Network connection direction.</span></span> <span data-ttu-id="dc52d-129">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="dc52d-129">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="dc52d-130">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="dc52d-130">domainRegisteredDateTime</span></span>|<span data-ttu-id="dc52d-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc52d-131">DateTimeOffset</span></span>|<span data-ttu-id="dc52d-132">Data quando o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="dc52d-132">Date when the destination domain was registered.</span></span> <span data-ttu-id="dc52d-133">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="dc52d-133">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="dc52d-134">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dc52d-134">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dc52d-135">localDnsName</span><span class="sxs-lookup"><span data-stu-id="dc52d-135">localDnsName</span></span>|<span data-ttu-id="dc52d-136">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-136">String</span></span>|<span data-ttu-id="dc52d-137">O local a resolução de nomes DNS como ele aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' foi violado).</span><span class="sxs-lookup"><span data-stu-id="dc52d-137">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="dc52d-138">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="dc52d-138">natDestinationAddress</span></span>|<span data-ttu-id="dc52d-139">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-139">String</span></span>|<span data-ttu-id="dc52d-140">Endereço IP de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-140">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="dc52d-141">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="dc52d-141">natDestinationPort</span></span>|<span data-ttu-id="dc52d-142">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-142">String</span></span>|<span data-ttu-id="dc52d-143">Porta de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-143">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="dc52d-144">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="dc52d-144">natSourceAddress</span></span>|<span data-ttu-id="dc52d-145">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-145">String</span></span>|<span data-ttu-id="dc52d-146">Endereço IP de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-146">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="dc52d-147">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="dc52d-147">natSourcePort</span></span>|<span data-ttu-id="dc52d-148">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-148">String</span></span>|<span data-ttu-id="dc52d-149">Porta de origem da conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-149">Network Address Translation source port.</span></span>|
|<span data-ttu-id="dc52d-150">protocolo</span><span class="sxs-lookup"><span data-stu-id="dc52d-150">protocol</span></span>|[<span data-ttu-id="dc52d-151">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="dc52d-151">securityNetworkProtocol</span></span>](securitynetworkprotocol.md)|<span data-ttu-id="dc52d-152">Protocolo de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-152">Network protocol.</span></span> <span data-ttu-id="dc52d-153">Os valores possíveis são: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="dc52d-153">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="dc52d-154">riskScore</span><span class="sxs-lookup"><span data-stu-id="dc52d-154">riskScore</span></span>|<span data-ttu-id="dc52d-155">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-155">String</span></span>|<span data-ttu-id="dc52d-156">Provedor gerado/calculado o risco de pontuação de conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-156">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="dc52d-157">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="dc52d-157">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="dc52d-158">Endereço_da_origem</span><span class="sxs-lookup"><span data-stu-id="dc52d-158">sourceAddress</span></span>|<span data-ttu-id="dc52d-159">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-159">String</span></span>|<span data-ttu-id="dc52d-160">Endereço IP de origem (isto é, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="dc52d-160">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="dc52d-161">Porta_da_origem</span><span class="sxs-lookup"><span data-stu-id="dc52d-161">sourcePort</span></span>|<span data-ttu-id="dc52d-162">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-162">String</span></span>|<span data-ttu-id="dc52d-163">Porta de IP de origem (isto é, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="dc52d-163">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="dc52d-164">status</span><span class="sxs-lookup"><span data-stu-id="dc52d-164">status</span></span>|<span data-ttu-id="dc52d-165">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="dc52d-165">connectionStatus</span></span>|<span data-ttu-id="dc52d-166">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="dc52d-166">Network connection status.</span></span> <span data-ttu-id="dc52d-167">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="dc52d-167">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="dc52d-168">urlParameters</span><span class="sxs-lookup"><span data-stu-id="dc52d-168">urlParameters</span></span>|<span data-ttu-id="dc52d-169">String</span><span class="sxs-lookup"><span data-stu-id="dc52d-169">String</span></span>|<span data-ttu-id="dc52d-170">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="dc52d-170">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dc52d-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dc52d-171">JSON representation</span></span>

<span data-ttu-id="dc52d-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dc52d-172">The following is a JSON representation of the resource.</span></span>

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