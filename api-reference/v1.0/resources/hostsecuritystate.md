---
title: tipo de recurso hostSecurityState
description: Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: dabe7d0aa026cb1b514e95fbc953dcb1974f8925
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029271"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="57899-103">tipo de recurso hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="57899-103">hostSecurityState resource type</span></span>

<span data-ttu-id="57899-104">Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="57899-104">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="57899-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57899-105">Properties</span></span>

| <span data-ttu-id="57899-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57899-106">Property</span></span>   | <span data-ttu-id="57899-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="57899-107">Type</span></span>|<span data-ttu-id="57899-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="57899-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="57899-109">FQDN</span><span class="sxs-lookup"><span data-stu-id="57899-109">fqdn</span></span>|<span data-ttu-id="57899-110">String</span><span class="sxs-lookup"><span data-stu-id="57899-110">String</span></span>|<span data-ttu-id="57899-111">FQDN do host (nome de domínio totalmente qualificado) (por `machine.company.com`exemplo,).</span><span class="sxs-lookup"><span data-stu-id="57899-111">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="57899-112">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="57899-112">isAzureAadJoined</span></span>|<span data-ttu-id="57899-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="57899-113">Boolean</span></span>|<span data-ttu-id="57899-114">True se o host estiver associado ao domínio nos serviços de domínio do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57899-114">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="57899-115">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="57899-115">isAzureAadRegistered</span></span>|<span data-ttu-id="57899-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="57899-116">Boolean</span></span>|<span data-ttu-id="57899-117">True se o host registrado no registro de dispositivo do Azure Active Directory (dispositivos BYOD-ou seja, não é totalmente gerenciado pela empresa).</span><span class="sxs-lookup"><span data-stu-id="57899-117">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="57899-118">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="57899-118">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="57899-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="57899-119">Boolean</span></span>|<span data-ttu-id="57899-120">True se o host é membro de um domínio do Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="57899-120">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="57899-121">NetBiosName</span><span class="sxs-lookup"><span data-stu-id="57899-121">netBiosName</span></span>|<span data-ttu-id="57899-122">String</span><span class="sxs-lookup"><span data-stu-id="57899-122">String</span></span>|<span data-ttu-id="57899-123">O nome do host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="57899-123">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="57899-124">Opera</span><span class="sxs-lookup"><span data-stu-id="57899-124">os</span></span>|<span data-ttu-id="57899-125">String</span><span class="sxs-lookup"><span data-stu-id="57899-125">String</span></span>|<span data-ttu-id="57899-126">Sistema operacional host.</span><span class="sxs-lookup"><span data-stu-id="57899-126">Host Operating System.</span></span> <span data-ttu-id="57899-127">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="57899-127">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="57899-128">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="57899-128">privateIpAddress</span></span>|<span data-ttu-id="57899-129">String</span><span class="sxs-lookup"><span data-stu-id="57899-129">String</span></span>|<span data-ttu-id="57899-130">Privado (não roteável) endereço IPv4 ou IPv6 (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="57899-130">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="57899-131">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="57899-131">publicIpAddress</span></span>|<span data-ttu-id="57899-132">String</span><span class="sxs-lookup"><span data-stu-id="57899-132">String</span></span>|<span data-ttu-id="57899-133">Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="57899-133">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="57899-134">riskScore</span><span class="sxs-lookup"><span data-stu-id="57899-134">riskScore</span></span>|<span data-ttu-id="57899-135">String</span><span class="sxs-lookup"><span data-stu-id="57899-135">String</span></span>|<span data-ttu-id="57899-136">Pontuação de risco calculado/gerado pelo provedor do host.</span><span class="sxs-lookup"><span data-stu-id="57899-136">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="57899-137">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="57899-137">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="57899-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57899-138">JSON representation</span></span>

<span data-ttu-id="57899-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57899-139">The following is a JSON representation of the resource.</span></span>

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
