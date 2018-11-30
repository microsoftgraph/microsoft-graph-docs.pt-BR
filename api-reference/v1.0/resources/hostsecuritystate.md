---
title: tipo de recurso de hostSecurityState
description: Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).
ms.openlocfilehash: 3649553ae0f96222a09825e8819dfd0d199f8454
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006227"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="d3c98-103">tipo de recurso de hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="d3c98-103">hostSecurityState resource type</span></span>

<span data-ttu-id="d3c98-104">Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="d3c98-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="d3c98-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d3c98-105">Properties</span></span>

| <span data-ttu-id="d3c98-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d3c98-106">Property</span></span>   | <span data-ttu-id="d3c98-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d3c98-107">Type</span></span>|<span data-ttu-id="d3c98-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d3c98-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d3c98-109">FQDN</span><span class="sxs-lookup"><span data-stu-id="d3c98-109">fqdn</span></span>|<span data-ttu-id="d3c98-110">String</span><span class="sxs-lookup"><span data-stu-id="d3c98-110">String</span></span>|<span data-ttu-id="d3c98-111">FQDN (nome de domínio totalmente qualificado) do host (por exemplo, `machine.company.com`).</span><span class="sxs-lookup"><span data-stu-id="d3c98-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="d3c98-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="d3c98-112">isAzureAadJoined</span></span>|<span data-ttu-id="d3c98-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3c98-113">Boolean</span></span>|<span data-ttu-id="d3c98-114">True se o host está integrado aos serviços de domínio do Azure Active Directory ao domínio.</span><span class="sxs-lookup"><span data-stu-id="d3c98-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="d3c98-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="d3c98-115">isAzureAadRegistered</span></span>|<span data-ttu-id="d3c98-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3c98-116">Boolean</span></span>|<span data-ttu-id="d3c98-117">True se o host registrado com o Windows Azure Active Directory dispositivo registro (BYOD dispositivos - ou seja, não totalmente gerenciados pelo enterprise).</span><span class="sxs-lookup"><span data-stu-id="d3c98-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="d3c98-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="d3c98-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="d3c98-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="d3c98-119">Boolean</span></span>|<span data-ttu-id="d3c98-120">True se o host é associado a um domínio do Active Directory no local de domínio.</span><span class="sxs-lookup"><span data-stu-id="d3c98-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="d3c98-121">Nome_netbios</span><span class="sxs-lookup"><span data-stu-id="d3c98-121">netBiosName</span></span>|<span data-ttu-id="d3c98-122">String</span><span class="sxs-lookup"><span data-stu-id="d3c98-122">String</span></span>|<span data-ttu-id="d3c98-123">O nome de host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="d3c98-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="d3c98-124">sistema operacional</span><span class="sxs-lookup"><span data-stu-id="d3c98-124">os</span></span>|<span data-ttu-id="d3c98-125">String</span><span class="sxs-lookup"><span data-stu-id="d3c98-125">String</span></span>|<span data-ttu-id="d3c98-126">Sistema operacional do host.</span><span class="sxs-lookup"><span data-stu-id="d3c98-126">Host Operating System.</span></span> <span data-ttu-id="d3c98-127">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="d3c98-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="d3c98-128">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="d3c98-128">privateIpAddress</span></span>|<span data-ttu-id="d3c98-129">String</span><span class="sxs-lookup"><span data-stu-id="d3c98-129">String</span></span>|<span data-ttu-id="d3c98-130">Endereço IPv4 ou IPv6 (não pode ser roteado) particular (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="d3c98-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="d3c98-131">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="d3c98-131">publicIpAddress</span></span>|<span data-ttu-id="d3c98-132">String</span><span class="sxs-lookup"><span data-stu-id="d3c98-132">String</span></span>|<span data-ttu-id="d3c98-133">Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) em tempo de alerta.</span><span class="sxs-lookup"><span data-stu-id="d3c98-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="d3c98-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="d3c98-134">riskScore</span></span>|<span data-ttu-id="d3c98-135">String</span><span class="sxs-lookup"><span data-stu-id="d3c98-135">String</span></span>|<span data-ttu-id="d3c98-136">Pontuação de risco de provedor-gerado/calculado do host.</span><span class="sxs-lookup"><span data-stu-id="d3c98-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="d3c98-137">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="d3c98-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d3c98-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d3c98-138">JSON representation</span></span>

<span data-ttu-id="d3c98-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d3c98-139">The following is a JSON representation of the resource.</span></span>

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
