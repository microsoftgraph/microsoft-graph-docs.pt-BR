---
title: tipo de recurso networkConnection
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: 6d28149854ed3157473b678db442ee3474e456c6
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29571916"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="0b2bb-104">tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="0b2bb-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b2bb-105">Contém informações com informações de estado sobre a conexão de rede relacionado ao alerta.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="0b2bb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b2bb-106">Properties</span></span>

| <span data-ttu-id="0b2bb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b2bb-107">Property</span></span>   | <span data-ttu-id="0b2bb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b2bb-108">Type</span></span>|<span data-ttu-id="0b2bb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b2bb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b2bb-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="0b2bb-110">applicationName</span></span>|<span data-ttu-id="0b2bb-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0b2bb-111">String</span></span>|<span data-ttu-id="0b2bb-112">Nome do aplicativo de gerenciamento de conexão de rede (por exemplo, Facebook, SMTP, etc.).</span><span class="sxs-lookup"><span data-stu-id="0b2bb-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="0b2bb-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="0b2bb-113">destinationAddress</span></span>|<span data-ttu-id="0b2bb-114">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-114">String</span></span>|<span data-ttu-id="0b2bb-115">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="0b2bb-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="0b2bb-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="0b2bb-116">destinationDomain</span></span>|<span data-ttu-id="0b2bb-117">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-117">String</span></span>|<span data-ttu-id="0b2bb-118">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="0b2bb-119">(por exemplo 'www.contoso.com').</span><span class="sxs-lookup"><span data-stu-id="0b2bb-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="0b2bb-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="0b2bb-120">destinationPort</span></span>|<span data-ttu-id="0b2bb-121">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-121">String</span></span>|<span data-ttu-id="0b2bb-122">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="0b2bb-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="0b2bb-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="0b2bb-123">destinationUrl</span></span>|<span data-ttu-id="0b2bb-124">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-124">String</span></span>|<span data-ttu-id="0b2bb-125">Cadeia de caracteres de URL/URI de conexão - excluindo os parâmetros de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="0b2bb-126">(por exemplo, 'www.contoso.com/products/default.html')</span><span class="sxs-lookup"><span data-stu-id="0b2bb-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="0b2bb-127">direção</span><span class="sxs-lookup"><span data-stu-id="0b2bb-127">direction</span></span>|<span data-ttu-id="0b2bb-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="0b2bb-128">connectionDirection</span></span>|<span data-ttu-id="0b2bb-129">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-129">Network connection direction.</span></span> <span data-ttu-id="0b2bb-130">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="0b2bb-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="0b2bb-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="0b2bb-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b2bb-132">DateTimeOffset</span></span>|<span data-ttu-id="0b2bb-133">Data quando o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="0b2bb-134">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="0b2bb-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="0b2bb-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="0b2bb-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="0b2bb-136">localDnsName</span></span>|<span data-ttu-id="0b2bb-137">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-137">String</span></span>|<span data-ttu-id="0b2bb-138">O local a resolução de nomes DNS como ele aparece no cache DNS local do host (por exemplo, caso o arquivo 'hosts' foi violado).</span><span class="sxs-lookup"><span data-stu-id="0b2bb-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="0b2bb-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="0b2bb-139">natDestinationAddress</span></span>|<span data-ttu-id="0b2bb-140">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-140">String</span></span>|<span data-ttu-id="0b2bb-141">Endereço IP de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="0b2bb-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="0b2bb-142">natDestinationPort</span></span>|<span data-ttu-id="0b2bb-143">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-143">String</span></span>|<span data-ttu-id="0b2bb-144">Porta de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="0b2bb-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="0b2bb-145">natSourceAddress</span></span>|<span data-ttu-id="0b2bb-146">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-146">String</span></span>|<span data-ttu-id="0b2bb-147">Endereço IP de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="0b2bb-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="0b2bb-148">natSourcePort</span></span>|<span data-ttu-id="0b2bb-149">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-149">String</span></span>|<span data-ttu-id="0b2bb-150">Porta de origem da conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="0b2bb-151">protocolo</span><span class="sxs-lookup"><span data-stu-id="0b2bb-151">protocol</span></span>| <span data-ttu-id="0b2bb-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="0b2bb-152">securityNetworkProtocol</span></span> |<span data-ttu-id="0b2bb-153">Protocolo de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-153">Network protocol.</span></span> <span data-ttu-id="0b2bb-154">Os valores possíveis são: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="0b2bb-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="0b2bb-155">riskScore</span></span>|<span data-ttu-id="0b2bb-156">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-156">String</span></span>|<span data-ttu-id="0b2bb-157">Provedor gerado/calculado o risco de pontuação de conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="0b2bb-158">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="0b2bb-159">Endereço_da_origem</span><span class="sxs-lookup"><span data-stu-id="0b2bb-159">sourceAddress</span></span>|<span data-ttu-id="0b2bb-160">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-160">String</span></span>|<span data-ttu-id="0b2bb-161">Endereço IP de origem (isto é, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="0b2bb-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="0b2bb-162">Porta_da_origem</span><span class="sxs-lookup"><span data-stu-id="0b2bb-162">sourcePort</span></span>|<span data-ttu-id="0b2bb-163">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-163">String</span></span>|<span data-ttu-id="0b2bb-164">Porta de IP de origem (isto é, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="0b2bb-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="0b2bb-165">status</span><span class="sxs-lookup"><span data-stu-id="0b2bb-165">status</span></span>|<span data-ttu-id="0b2bb-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="0b2bb-166">connectionStatus</span></span>|<span data-ttu-id="0b2bb-167">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-167">Network connection status.</span></span> <span data-ttu-id="0b2bb-168">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="0b2bb-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="0b2bb-169">urlParameters</span></span>|<span data-ttu-id="0b2bb-170">String</span><span class="sxs-lookup"><span data-stu-id="0b2bb-170">String</span></span>|<span data-ttu-id="0b2bb-171">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b2bb-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b2bb-172">JSON representation</span></span>

<span data-ttu-id="0b2bb-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b2bb-173">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "networkConnection resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/networkconnection.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
