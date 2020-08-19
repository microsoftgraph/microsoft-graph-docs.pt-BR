---
title: tipo de recurso hostSecurityState
description: Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e358280e1c510a763a8fa38febce060448491270
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806083"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="efac6-103">tipo de recurso hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="efac6-103">hostSecurityState resource type</span></span>

<span data-ttu-id="efac6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efac6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efac6-105">Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="efac6-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="efac6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="efac6-106">Properties</span></span>

| <span data-ttu-id="efac6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="efac6-107">Property</span></span>   | <span data-ttu-id="efac6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="efac6-108">Type</span></span>|<span data-ttu-id="efac6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="efac6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="efac6-110">FQDN</span><span class="sxs-lookup"><span data-stu-id="efac6-110">fqdn</span></span>|<span data-ttu-id="efac6-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efac6-111">String</span></span>|<span data-ttu-id="efac6-112">FQDN do host (nome de domínio totalmente qualificado) (por exemplo, `machine.company.com` ).</span><span class="sxs-lookup"><span data-stu-id="efac6-112">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="efac6-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="efac6-113">isAzureAadJoined</span></span>|<span data-ttu-id="efac6-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="efac6-114">Boolean</span></span>|<span data-ttu-id="efac6-115">True se o host estiver associado ao domínio nos serviços de domínio do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="efac6-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="efac6-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="efac6-116">isAzureAadRegistered</span></span>|<span data-ttu-id="efac6-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="efac6-117">Boolean</span></span>|<span data-ttu-id="efac6-118">True se o host registrado no registro de dispositivo do Azure Active Directory (dispositivos BYOD-ou seja, não é totalmente gerenciado pela empresa).</span><span class="sxs-lookup"><span data-stu-id="efac6-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="efac6-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="efac6-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="efac6-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="efac6-120">Boolean</span></span>|<span data-ttu-id="efac6-121">True se o host é membro de um domínio do Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="efac6-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="efac6-122">NetBiosName</span><span class="sxs-lookup"><span data-stu-id="efac6-122">netBiosName</span></span>|<span data-ttu-id="efac6-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efac6-123">String</span></span>|<span data-ttu-id="efac6-124">O nome do host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="efac6-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="efac6-125">Opera</span><span class="sxs-lookup"><span data-stu-id="efac6-125">os</span></span>|<span data-ttu-id="efac6-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efac6-126">String</span></span>|<span data-ttu-id="efac6-127">Sistema operacional host.</span><span class="sxs-lookup"><span data-stu-id="efac6-127">Host Operating System.</span></span> <span data-ttu-id="efac6-128">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="efac6-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="efac6-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="efac6-129">privateIpAddress</span></span>|<span data-ttu-id="efac6-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efac6-130">String</span></span>|<span data-ttu-id="efac6-131">Privado (não roteável) endereço IPv4 ou IPv6 (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="efac6-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="efac6-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="efac6-132">publicIpAddress</span></span>|<span data-ttu-id="efac6-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efac6-133">String</span></span>|<span data-ttu-id="efac6-134">Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="efac6-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="efac6-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="efac6-135">riskScore</span></span>|<span data-ttu-id="efac6-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="efac6-136">String</span></span>|<span data-ttu-id="efac6-137">Pontuação de risco calculado/gerado pelo provedor do host.</span><span class="sxs-lookup"><span data-stu-id="efac6-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="efac6-138">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="efac6-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="efac6-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="efac6-139">JSON representation</span></span>

<span data-ttu-id="efac6-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="efac6-140">The following is a JSON representation of the resource.</span></span>

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
