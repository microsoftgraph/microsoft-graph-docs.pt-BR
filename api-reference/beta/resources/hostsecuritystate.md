---
title: tipo de recurso de hostSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
ms.openlocfilehash: ae64d4e0f13e39cb344fd54f5e600cfbfe0dc4f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036561"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="c0472-104">tipo de recurso de hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="c0472-104">hostSecurityState resource type</span></span>

 > <span data-ttu-id="c0472-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c0472-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0472-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c0472-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c0472-107">Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="c0472-107">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="c0472-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c0472-108">Properties</span></span>

| <span data-ttu-id="c0472-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c0472-109">Property</span></span>   | <span data-ttu-id="c0472-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c0472-110">Type</span></span>|<span data-ttu-id="c0472-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0472-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c0472-112">FQDN</span><span class="sxs-lookup"><span data-stu-id="c0472-112">fqdn</span></span>|<span data-ttu-id="c0472-113">String</span><span class="sxs-lookup"><span data-stu-id="c0472-113">String</span></span>|<span data-ttu-id="c0472-114">O FQDN (nome totalmente qualificado) (por exemplo, machine.company.com) do host.</span><span class="sxs-lookup"><span data-stu-id="c0472-114">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="c0472-115">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="c0472-115">isAzureAadJoined</span></span>|<span data-ttu-id="c0472-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0472-116">Boolean</span></span>|<span data-ttu-id="c0472-117">True se o host está integrado aos serviços de domínio do Azure Active Directory ao domínio.</span><span class="sxs-lookup"><span data-stu-id="c0472-117">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="c0472-118">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="c0472-118">isAzureAadRegistered</span></span>|<span data-ttu-id="c0472-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0472-119">Boolean</span></span>|<span data-ttu-id="c0472-120">True se o host registrado com o Windows Azure Active Directory dispositivo registro (BYOD dispositivos - ou seja, não totalmente gerenciados pelo enterprise).</span><span class="sxs-lookup"><span data-stu-id="c0472-120">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="c0472-121">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="c0472-121">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="c0472-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="c0472-122">Boolean</span></span>|<span data-ttu-id="c0472-123">True se o host é associado a um domínio do Active Directory no local de domínio.</span><span class="sxs-lookup"><span data-stu-id="c0472-123">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="c0472-124">Nome_netbios</span><span class="sxs-lookup"><span data-stu-id="c0472-124">netBiosName</span></span>|<span data-ttu-id="c0472-125">String</span><span class="sxs-lookup"><span data-stu-id="c0472-125">String</span></span>|<span data-ttu-id="c0472-126">O nome de host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="c0472-126">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="c0472-127">sistema operacional</span><span class="sxs-lookup"><span data-stu-id="c0472-127">os</span></span>|<span data-ttu-id="c0472-128">String</span><span class="sxs-lookup"><span data-stu-id="c0472-128">String</span></span>|<span data-ttu-id="c0472-129">Sistema operacional do host.</span><span class="sxs-lookup"><span data-stu-id="c0472-129">Host Operating System.</span></span> <span data-ttu-id="c0472-130">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="c0472-130">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="c0472-131">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="c0472-131">privateIpAddress</span></span>|<span data-ttu-id="c0472-132">String</span><span class="sxs-lookup"><span data-stu-id="c0472-132">String</span></span>|<span data-ttu-id="c0472-133">Endereço IPv4 ou IPv6 (não pode ser roteado) particular (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="c0472-133">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="c0472-134">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="c0472-134">publicIpAddress</span></span>|<span data-ttu-id="c0472-135">String</span><span class="sxs-lookup"><span data-stu-id="c0472-135">String</span></span>|<span data-ttu-id="c0472-136">Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) em tempo de alerta.</span><span class="sxs-lookup"><span data-stu-id="c0472-136">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="c0472-137">riskScore</span><span class="sxs-lookup"><span data-stu-id="c0472-137">riskScore</span></span>|<span data-ttu-id="c0472-138">String</span><span class="sxs-lookup"><span data-stu-id="c0472-138">String</span></span>|<span data-ttu-id="c0472-139">Pontuação de risco de provedor-gerado/calculado do host.</span><span class="sxs-lookup"><span data-stu-id="c0472-139">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="c0472-140">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="c0472-140">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c0472-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c0472-141">JSON representation</span></span>

<span data-ttu-id="c0472-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c0472-142">The following is a JSON representation of the resource.</span></span>

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
