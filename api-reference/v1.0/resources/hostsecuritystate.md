---
title: tipo de recurso hostSecurityState
description: Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 2d8543512162398f38f9ddb74cf72f57171c58f8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48062880"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="8ffb0-103">tipo de recurso hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="8ffb0-103">hostSecurityState resource type</span></span>

<span data-ttu-id="8ffb0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ffb0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8ffb0-105">Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="8ffb0-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="8ffb0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ffb0-106">Properties</span></span>

| <span data-ttu-id="8ffb0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ffb0-107">Property</span></span>   | <span data-ttu-id="8ffb0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ffb0-108">Type</span></span>|<span data-ttu-id="8ffb0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ffb0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ffb0-110">FQDN</span><span class="sxs-lookup"><span data-stu-id="8ffb0-110">fqdn</span></span>|<span data-ttu-id="8ffb0-111">String</span><span class="sxs-lookup"><span data-stu-id="8ffb0-111">String</span></span>|<span data-ttu-id="8ffb0-112">FQDN do host (nome de domínio totalmente qualificado) (por exemplo, `machine.company.com` ).</span><span class="sxs-lookup"><span data-stu-id="8ffb0-112">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="8ffb0-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="8ffb0-113">isAzureAadJoined</span></span>|<span data-ttu-id="8ffb0-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ffb0-114">Boolean</span></span>|<span data-ttu-id="8ffb0-115">True se o host estiver associado ao domínio nos serviços de domínio do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="8ffb0-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="8ffb0-116">isAzureAadRegistered</span></span>|<span data-ttu-id="8ffb0-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ffb0-117">Boolean</span></span>|<span data-ttu-id="8ffb0-118">True se o host registrado no registro de dispositivo do Azure Active Directory (dispositivos BYOD-ou seja, não é totalmente gerenciado pela empresa).</span><span class="sxs-lookup"><span data-stu-id="8ffb0-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="8ffb0-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="8ffb0-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="8ffb0-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ffb0-120">Boolean</span></span>|<span data-ttu-id="8ffb0-121">True se o host é membro de um domínio do Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="8ffb0-122">NetBiosName</span><span class="sxs-lookup"><span data-stu-id="8ffb0-122">netBiosName</span></span>|<span data-ttu-id="8ffb0-123">String</span><span class="sxs-lookup"><span data-stu-id="8ffb0-123">String</span></span>|<span data-ttu-id="8ffb0-124">O nome do host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="8ffb0-125">Opera</span><span class="sxs-lookup"><span data-stu-id="8ffb0-125">os</span></span>|<span data-ttu-id="8ffb0-126">String</span><span class="sxs-lookup"><span data-stu-id="8ffb0-126">String</span></span>|<span data-ttu-id="8ffb0-127">Sistema operacional host.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-127">Host Operating System.</span></span> <span data-ttu-id="8ffb0-128">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="8ffb0-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="8ffb0-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="8ffb0-129">privateIpAddress</span></span>|<span data-ttu-id="8ffb0-130">String</span><span class="sxs-lookup"><span data-stu-id="8ffb0-130">String</span></span>|<span data-ttu-id="8ffb0-131">Privado (não roteável) endereço IPv4 ou IPv6 (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="8ffb0-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="8ffb0-132">publicIpAddress</span></span>|<span data-ttu-id="8ffb0-133">String</span><span class="sxs-lookup"><span data-stu-id="8ffb0-133">String</span></span>|<span data-ttu-id="8ffb0-134">Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="8ffb0-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="8ffb0-135">riskScore</span></span>|<span data-ttu-id="8ffb0-136">String</span><span class="sxs-lookup"><span data-stu-id="8ffb0-136">String</span></span>|<span data-ttu-id="8ffb0-137">Pontuação de risco calculado/gerado pelo provedor do host.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="8ffb0-138">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ffb0-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ffb0-139">JSON representation</span></span>

<span data-ttu-id="8ffb0-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ffb0-140">The following is a JSON representation of the resource.</span></span>

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

