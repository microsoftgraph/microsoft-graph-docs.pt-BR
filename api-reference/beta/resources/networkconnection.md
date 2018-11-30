---
title: tipo de recurso networkConnection
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: 7dfc055c7603adc8d60908df58ce3995927316cd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039313"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="5b440-104">tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="5b440-104">networkConnection resource type</span></span>

 > <span data-ttu-id="5b440-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="5b440-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b440-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5b440-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5b440-107">Contém informações com informações de estado sobre a conexão de rede relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="5b440-107">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="5b440-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b440-108">Properties</span></span>

| <span data-ttu-id="5b440-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b440-109">Property</span></span>   | <span data-ttu-id="5b440-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b440-110">Type</span></span>|<span data-ttu-id="5b440-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b440-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5b440-112">applicationName</span><span class="sxs-lookup"><span data-stu-id="5b440-112">applicationName</span></span>|<span data-ttu-id="5b440-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b440-113">String</span></span>|<span data-ttu-id="5b440-114">Nome do aplicativo de gerenciamento de conexão de rede (por exemplo, Facebook, SMTP, etc.).</span><span class="sxs-lookup"><span data-stu-id="5b440-114">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="5b440-115">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="5b440-115">destinationAddress</span></span>|<span data-ttu-id="5b440-116">String</span><span class="sxs-lookup"><span data-stu-id="5b440-116">String</span></span>|<span data-ttu-id="5b440-117">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="5b440-117">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="5b440-118">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="5b440-118">destinationDomain</span></span>|<span data-ttu-id="5b440-119">String</span><span class="sxs-lookup"><span data-stu-id="5b440-119">String</span></span>|<span data-ttu-id="5b440-120">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="5b440-120">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="5b440-121">(por exemplo 'www.contoso.com').</span><span class="sxs-lookup"><span data-stu-id="5b440-121">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="5b440-122">destinationPort</span><span class="sxs-lookup"><span data-stu-id="5b440-122">destinationPort</span></span>|<span data-ttu-id="5b440-123">String</span><span class="sxs-lookup"><span data-stu-id="5b440-123">String</span></span>|<span data-ttu-id="5b440-124">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="5b440-124">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="5b440-125">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="5b440-125">destinationUrl</span></span>|<span data-ttu-id="5b440-126">String</span><span class="sxs-lookup"><span data-stu-id="5b440-126">String</span></span>|<span data-ttu-id="5b440-127">Cadeia de caracteres de URL/URI de conexão - excluindo os parâmetros de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-127">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="5b440-128">(por exemplo, 'www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="5b440-128">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="5b440-129">direção</span><span class="sxs-lookup"><span data-stu-id="5b440-129">direction</span></span>|<span data-ttu-id="5b440-130">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="5b440-130">connectionDirection</span></span>|<span data-ttu-id="5b440-131">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-131">Network connection direction.</span></span> <span data-ttu-id="5b440-132">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="5b440-132">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="5b440-133">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="5b440-133">domainRegisteredDateTime</span></span>|<span data-ttu-id="5b440-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b440-134">DateTimeOffset</span></span>|<span data-ttu-id="5b440-135">Data quando o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="5b440-135">Date when the destination domain was registered.</span></span> <span data-ttu-id="5b440-136">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="5b440-136">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="5b440-137">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="5b440-137">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="5b440-138">localDnsName</span><span class="sxs-lookup"><span data-stu-id="5b440-138">localDnsName</span></span>|<span data-ttu-id="5b440-139">String</span><span class="sxs-lookup"><span data-stu-id="5b440-139">String</span></span>|<span data-ttu-id="5b440-140">O local a resolução de nomes DNS como ele aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' foi violado).</span><span class="sxs-lookup"><span data-stu-id="5b440-140">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="5b440-141">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="5b440-141">natDestinationAddress</span></span>|<span data-ttu-id="5b440-142">String</span><span class="sxs-lookup"><span data-stu-id="5b440-142">String</span></span>|<span data-ttu-id="5b440-143">Endereço IP de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-143">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="5b440-144">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="5b440-144">natDestinationPort</span></span>|<span data-ttu-id="5b440-145">String</span><span class="sxs-lookup"><span data-stu-id="5b440-145">String</span></span>|<span data-ttu-id="5b440-146">Porta de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-146">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="5b440-147">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="5b440-147">natSourceAddress</span></span>|<span data-ttu-id="5b440-148">String</span><span class="sxs-lookup"><span data-stu-id="5b440-148">String</span></span>|<span data-ttu-id="5b440-149">Endereço IP de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-149">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="5b440-150">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="5b440-150">natSourcePort</span></span>|<span data-ttu-id="5b440-151">String</span><span class="sxs-lookup"><span data-stu-id="5b440-151">String</span></span>|<span data-ttu-id="5b440-152">Porta de origem da conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-152">Network Address Translation source port.</span></span>|
|<span data-ttu-id="5b440-153">protocolo</span><span class="sxs-lookup"><span data-stu-id="5b440-153">protocol</span></span>|[<span data-ttu-id="5b440-154">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="5b440-154">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="5b440-155">Protocolo de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-155">Network protocol.</span></span> <span data-ttu-id="5b440-156">Os valores possíveis são: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="5b440-156">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="5b440-157">riskScore</span><span class="sxs-lookup"><span data-stu-id="5b440-157">riskScore</span></span>|<span data-ttu-id="5b440-158">String</span><span class="sxs-lookup"><span data-stu-id="5b440-158">String</span></span>|<span data-ttu-id="5b440-159">Provedor gerado/calculado o risco de pontuação de conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-159">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="5b440-160">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="5b440-160">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="5b440-161">Endereço_da_origem</span><span class="sxs-lookup"><span data-stu-id="5b440-161">sourceAddress</span></span>|<span data-ttu-id="5b440-162">String</span><span class="sxs-lookup"><span data-stu-id="5b440-162">String</span></span>|<span data-ttu-id="5b440-163">Endereço IP de origem (isto é, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="5b440-163">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="5b440-164">Porta_da_origem</span><span class="sxs-lookup"><span data-stu-id="5b440-164">sourcePort</span></span>|<span data-ttu-id="5b440-165">String</span><span class="sxs-lookup"><span data-stu-id="5b440-165">String</span></span>|<span data-ttu-id="5b440-166">Porta de IP de origem (isto é, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="5b440-166">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="5b440-167">status</span><span class="sxs-lookup"><span data-stu-id="5b440-167">status</span></span>|<span data-ttu-id="5b440-168">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="5b440-168">connectionStatus</span></span>|<span data-ttu-id="5b440-169">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="5b440-169">Network connection status.</span></span> <span data-ttu-id="5b440-170">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="5b440-170">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="5b440-171">urlParameters</span><span class="sxs-lookup"><span data-stu-id="5b440-171">urlParameters</span></span>|<span data-ttu-id="5b440-172">String</span><span class="sxs-lookup"><span data-stu-id="5b440-172">String</span></span>|<span data-ttu-id="5b440-173">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="5b440-173">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5b440-174">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b440-174">JSON representation</span></span>

<span data-ttu-id="5b440-175">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b440-175">The following is a JSON representation of the resource.</span></span>

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
