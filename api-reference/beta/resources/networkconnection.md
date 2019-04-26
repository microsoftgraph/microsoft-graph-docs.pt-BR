---
title: tipo de recurso networkConnection
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: ce7de8d5a0f63c4d924e8092e4e9e05f984ec335
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570719"
---
# <a name="networkconnection-resource-type"></a><span data-ttu-id="f99dd-104">tipo de recurso networkConnection</span><span class="sxs-lookup"><span data-stu-id="f99dd-104">networkConnection resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f99dd-105">Contém informações de estado sobre a conexão de rede relacionada ao alerta.</span><span class="sxs-lookup"><span data-stu-id="f99dd-105">Contains stateful information about the network connection related to the alert.</span></span>

## <a name="properties"></a><span data-ttu-id="f99dd-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f99dd-106">Properties</span></span>

| <span data-ttu-id="f99dd-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f99dd-107">Property</span></span>   | <span data-ttu-id="f99dd-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f99dd-108">Type</span></span>|<span data-ttu-id="f99dd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f99dd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f99dd-110">applicationName</span><span class="sxs-lookup"><span data-stu-id="f99dd-110">applicationName</span></span>|<span data-ttu-id="f99dd-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f99dd-111">String</span></span>|<span data-ttu-id="f99dd-112">Nome do aplicativo que gerencia a conexão de rede (por exemplo, Facebook, SMTP, etc.).</span><span class="sxs-lookup"><span data-stu-id="f99dd-112">Name of the application managing the network connection (for example, Facebook, SMTP, etc.).</span></span>|
|<span data-ttu-id="f99dd-113">destinationAddress</span><span class="sxs-lookup"><span data-stu-id="f99dd-113">destinationAddress</span></span>|<span data-ttu-id="f99dd-114">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-114">String</span></span>|<span data-ttu-id="f99dd-115">Endereço IP de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="f99dd-115">Destination IP address (of the network connection).</span></span>|
|<span data-ttu-id="f99dd-116">destinationDomain</span><span class="sxs-lookup"><span data-stu-id="f99dd-116">destinationDomain</span></span>|<span data-ttu-id="f99dd-117">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-117">String</span></span>|<span data-ttu-id="f99dd-118">Parte do domínio de destino da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="f99dd-118">Destination domain portion of the destination URL.</span></span> <span data-ttu-id="f99dd-119">(por exemplo, ' www.contoso.com ').</span><span class="sxs-lookup"><span data-stu-id="f99dd-119">(for example 'www.contoso.com').</span></span>|
|<span data-ttu-id="f99dd-120">destinationPort</span><span class="sxs-lookup"><span data-stu-id="f99dd-120">destinationPort</span></span>|<span data-ttu-id="f99dd-121">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-121">String</span></span>|<span data-ttu-id="f99dd-122">Porta de destino (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="f99dd-122">Destination port (of the network connection).</span></span>|
|<span data-ttu-id="f99dd-123">destinationUrl</span><span class="sxs-lookup"><span data-stu-id="f99dd-123">destinationUrl</span></span>|<span data-ttu-id="f99dd-124">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-124">String</span></span>|<span data-ttu-id="f99dd-125">URL de conexão de rede/cadeia de caracteres URI-excluindo parâmetros.</span><span class="sxs-lookup"><span data-stu-id="f99dd-125">Network connection URL/URI string - excluding parameters.</span></span> <span data-ttu-id="f99dd-126">(por exemplo, ' www.contoso.com/products/default.html ')</span><span class="sxs-lookup"><span data-stu-id="f99dd-126">(for example 'www.contoso.com/products/default.html')</span></span>|
|<span data-ttu-id="f99dd-127">direction</span><span class="sxs-lookup"><span data-stu-id="f99dd-127">direction</span></span>|<span data-ttu-id="f99dd-128">connectionDirection</span><span class="sxs-lookup"><span data-stu-id="f99dd-128">connectionDirection</span></span>|<span data-ttu-id="f99dd-129">Direção da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-129">Network connection direction.</span></span> <span data-ttu-id="f99dd-130">Os valores possíveis são: `unknown`, `inbound`, `outbound`.</span><span class="sxs-lookup"><span data-stu-id="f99dd-130">Possible values are: `unknown`, `inbound`, `outbound`.</span></span>|
|<span data-ttu-id="f99dd-131">domainRegisteredDateTime</span><span class="sxs-lookup"><span data-stu-id="f99dd-131">domainRegisteredDateTime</span></span>|<span data-ttu-id="f99dd-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f99dd-132">DateTimeOffset</span></span>|<span data-ttu-id="f99dd-133">Data em que o domínio de destino foi registrado.</span><span class="sxs-lookup"><span data-stu-id="f99dd-133">Date when the destination domain was registered.</span></span> <span data-ttu-id="f99dd-134">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="f99dd-134">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f99dd-135">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f99dd-135">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f99dd-136">localDnsName</span><span class="sxs-lookup"><span data-stu-id="f99dd-136">localDnsName</span></span>|<span data-ttu-id="f99dd-137">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-137">String</span></span>|<span data-ttu-id="f99dd-138">A resolução de nome DNS local da forma como aparece no cache de DNS local do host (por exemplo, caso o arquivo "hosts" tenha sido adulterado).</span><span class="sxs-lookup"><span data-stu-id="f99dd-138">The local DNS name resolution as it appears in the host's local DNS cache (for example, in case the 'hosts' file was tampered with).</span></span>|
|<span data-ttu-id="f99dd-139">natDestinationAddress</span><span class="sxs-lookup"><span data-stu-id="f99dd-139">natDestinationAddress</span></span>|<span data-ttu-id="f99dd-140">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-140">String</span></span>|<span data-ttu-id="f99dd-141">Endereço IP de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-141">Network Address Translation destination IP address.</span></span>|
|<span data-ttu-id="f99dd-142">natDestinationPort</span><span class="sxs-lookup"><span data-stu-id="f99dd-142">natDestinationPort</span></span>|<span data-ttu-id="f99dd-143">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-143">String</span></span>|<span data-ttu-id="f99dd-144">Porta de destino de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-144">Network Address Translation destination port.</span></span>|
|<span data-ttu-id="f99dd-145">natSourceAddress</span><span class="sxs-lookup"><span data-stu-id="f99dd-145">natSourceAddress</span></span>|<span data-ttu-id="f99dd-146">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-146">String</span></span>|<span data-ttu-id="f99dd-147">Endereço IP de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-147">Network Address Translation source IP address.</span></span>|
|<span data-ttu-id="f99dd-148">natSourcePort</span><span class="sxs-lookup"><span data-stu-id="f99dd-148">natSourcePort</span></span>|<span data-ttu-id="f99dd-149">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-149">String</span></span>|<span data-ttu-id="f99dd-150">Porta de origem de conversão de endereço de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-150">Network Address Translation source port.</span></span>|
|<span data-ttu-id="f99dd-151">RDP</span><span class="sxs-lookup"><span data-stu-id="f99dd-151">protocol</span></span>|[<span data-ttu-id="f99dd-152">securityNetworkProtocol</span><span class="sxs-lookup"><span data-stu-id="f99dd-152">securityNetworkProtocol</span></span>](securitynetworkprotocolenumtype.md)|<span data-ttu-id="f99dd-153">Protocolo de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-153">Network protocol.</span></span> <span data-ttu-id="f99dd-154">Os valores possíveis são `unknown`: `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp` `ipv6` `ipv6RoutingHeader`,,, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd` ,,,,,,,, , `raw`, `ipx`, `spx`, `spxII`.</span><span class="sxs-lookup"><span data-stu-id="f99dd-154">Possible values are: `unknown`, `ip`, `icmp`, `igmp`, `ggp`, `ipv4`, `tcp`, `pup`, `udp`, `idp`, `ipv6`, `ipv6RoutingHeader`, `ipv6FragmentHeader`, `ipSecEncapsulatingSecurityPayload`, `ipSecAuthenticationHeader`, `icmpV6`, `ipv6NoNextHeader`, `ipv6DestinationOptions`, `nd`, `raw`, `ipx`, `spx`, `spxII`.</span></span>|
|<span data-ttu-id="f99dd-155">riskScore</span><span class="sxs-lookup"><span data-stu-id="f99dd-155">riskScore</span></span>|<span data-ttu-id="f99dd-156">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-156">String</span></span>|<span data-ttu-id="f99dd-157">Provedor gerado/Pontuação de risco calculado da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-157">Provider generated/calculated risk score of the network connection.</span></span> <span data-ttu-id="f99dd-158">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="f99dd-158">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="f99dd-159">sourceAddress</span><span class="sxs-lookup"><span data-stu-id="f99dd-159">sourceAddress</span></span>|<span data-ttu-id="f99dd-160">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-160">String</span></span>|<span data-ttu-id="f99dd-161">Endereço IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="f99dd-161">Source (i.e. origin) IP address (of the network connection).</span></span>|
|<span data-ttu-id="f99dd-162">sourcePort</span><span class="sxs-lookup"><span data-stu-id="f99dd-162">sourcePort</span></span>|<span data-ttu-id="f99dd-163">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-163">String</span></span>|<span data-ttu-id="f99dd-164">Porta IP de origem (ou seja, origem) (da conexão de rede).</span><span class="sxs-lookup"><span data-stu-id="f99dd-164">Source (i.e. origin) IP port (of the network connection).</span></span>|
|<span data-ttu-id="f99dd-165">status</span><span class="sxs-lookup"><span data-stu-id="f99dd-165">status</span></span>|<span data-ttu-id="f99dd-166">connectionStatus</span><span class="sxs-lookup"><span data-stu-id="f99dd-166">connectionStatus</span></span>|<span data-ttu-id="f99dd-167">Status da conexão de rede.</span><span class="sxs-lookup"><span data-stu-id="f99dd-167">Network connection status.</span></span> <span data-ttu-id="f99dd-168">Os valores possíveis são: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span><span class="sxs-lookup"><span data-stu-id="f99dd-168">Possible values are: `unknown`, `attempted`, `succeeded`, `blocked`, `failed`.</span></span>|
|<span data-ttu-id="f99dd-169">urlParameters</span><span class="sxs-lookup"><span data-stu-id="f99dd-169">urlParameters</span></span>|<span data-ttu-id="f99dd-170">String</span><span class="sxs-lookup"><span data-stu-id="f99dd-170">String</span></span>|<span data-ttu-id="f99dd-171">Parâmetros (sufixo) da URL de destino.</span><span class="sxs-lookup"><span data-stu-id="f99dd-171">Parameters (suffix) of the destination URL.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f99dd-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f99dd-172">JSON representation</span></span>

<span data-ttu-id="f99dd-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f99dd-173">The following is a JSON representation of the resource.</span></span>

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
