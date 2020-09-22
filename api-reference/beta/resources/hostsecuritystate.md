---
title: tipo de recurso hostSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: a76797ed5660a80e1bbce73609617844de326863
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013591"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="82950-104">tipo de recurso hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="82950-104">hostSecurityState resource type</span></span>

<span data-ttu-id="82950-105">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="82950-105">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82950-106">Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="82950-106">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="82950-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82950-107">Properties</span></span>

| <span data-ttu-id="82950-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82950-108">Property</span></span>   | <span data-ttu-id="82950-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="82950-109">Type</span></span>|<span data-ttu-id="82950-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="82950-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82950-111">FQDN</span><span class="sxs-lookup"><span data-stu-id="82950-111">fqdn</span></span>|<span data-ttu-id="82950-112">String</span><span class="sxs-lookup"><span data-stu-id="82950-112">String</span></span>|<span data-ttu-id="82950-113">FQDN do host (nome de domínio totalmente qualificado) (por exemplo, machine.company.com).</span><span class="sxs-lookup"><span data-stu-id="82950-113">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="82950-114">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="82950-114">isAzureAadJoined</span></span>|<span data-ttu-id="82950-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="82950-115">Boolean</span></span>|<span data-ttu-id="82950-116">True se o host estiver associado ao domínio nos serviços de domínio do Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="82950-116">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="82950-117">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="82950-117">isAzureAadRegistered</span></span>|<span data-ttu-id="82950-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="82950-118">Boolean</span></span>|<span data-ttu-id="82950-119">True se o host registrado no registro de dispositivo do Azure Active Directory (dispositivos BYOD-ou seja, não é totalmente gerenciado pela empresa).</span><span class="sxs-lookup"><span data-stu-id="82950-119">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="82950-120">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="82950-120">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="82950-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="82950-121">Boolean</span></span>|<span data-ttu-id="82950-122">True se o host é membro de um domínio do Active Directory local.</span><span class="sxs-lookup"><span data-stu-id="82950-122">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="82950-123">NetBiosName</span><span class="sxs-lookup"><span data-stu-id="82950-123">netBiosName</span></span>|<span data-ttu-id="82950-124">String</span><span class="sxs-lookup"><span data-stu-id="82950-124">String</span></span>|<span data-ttu-id="82950-125">O nome do host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="82950-125">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="82950-126">Opera</span><span class="sxs-lookup"><span data-stu-id="82950-126">os</span></span>|<span data-ttu-id="82950-127">String</span><span class="sxs-lookup"><span data-stu-id="82950-127">String</span></span>|<span data-ttu-id="82950-128">Sistema operacional host.</span><span class="sxs-lookup"><span data-stu-id="82950-128">Host Operating System.</span></span> <span data-ttu-id="82950-129">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="82950-129">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="82950-130">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="82950-130">privateIpAddress</span></span>|<span data-ttu-id="82950-131">String</span><span class="sxs-lookup"><span data-stu-id="82950-131">String</span></span>|<span data-ttu-id="82950-132">Privado (não roteável) endereço IPv4 ou IPv6 (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="82950-132">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="82950-133">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="82950-133">publicIpAddress</span></span>|<span data-ttu-id="82950-134">String</span><span class="sxs-lookup"><span data-stu-id="82950-134">String</span></span>|<span data-ttu-id="82950-135">Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="82950-135">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="82950-136">riskScore</span><span class="sxs-lookup"><span data-stu-id="82950-136">riskScore</span></span>|<span data-ttu-id="82950-137">String</span><span class="sxs-lookup"><span data-stu-id="82950-137">String</span></span>|<span data-ttu-id="82950-138">Pontuação de risco calculado/gerado pelo provedor do host.</span><span class="sxs-lookup"><span data-stu-id="82950-138">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="82950-139">O intervalo de valor recomendado de 0-1, que é igual a uma porcentagem.</span><span class="sxs-lookup"><span data-stu-id="82950-139">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="82950-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82950-140">JSON representation</span></span>

<span data-ttu-id="82950-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82950-141">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


