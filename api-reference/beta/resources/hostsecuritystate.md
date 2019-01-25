---
title: tipo de recurso de hostSecurityState
description: " > **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção."
localization_priority: Normal
ms.openlocfilehash: d6f566a2bd42163c570fe837d2419057c62664bb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526694"
---
# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="585c9-104">tipo de recurso de hostSecurityState</span><span class="sxs-lookup"><span data-stu-id="585c9-104">hostSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="585c9-105">Contém informações de estado sobre o host (incluindo dispositivos, computadores e assim por diante).</span><span class="sxs-lookup"><span data-stu-id="585c9-105">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="585c9-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="585c9-106">Properties</span></span>

| <span data-ttu-id="585c9-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="585c9-107">Property</span></span>   | <span data-ttu-id="585c9-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="585c9-108">Type</span></span>|<span data-ttu-id="585c9-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="585c9-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="585c9-110">FQDN</span><span class="sxs-lookup"><span data-stu-id="585c9-110">fqdn</span></span>|<span data-ttu-id="585c9-111">String</span><span class="sxs-lookup"><span data-stu-id="585c9-111">String</span></span>|<span data-ttu-id="585c9-112">O FQDN (nome totalmente qualificado) (por exemplo, machine.company.com) do host.</span><span class="sxs-lookup"><span data-stu-id="585c9-112">Host FQDN (Fully Qualified Domain Name) (for example, machine.company.com).</span></span>|
|<span data-ttu-id="585c9-113">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="585c9-113">isAzureAadJoined</span></span>|<span data-ttu-id="585c9-114">Booliano</span><span class="sxs-lookup"><span data-stu-id="585c9-114">Boolean</span></span>|<span data-ttu-id="585c9-115">True se o host está integrado aos serviços de domínio do Azure Active Directory ao domínio.</span><span class="sxs-lookup"><span data-stu-id="585c9-115">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="585c9-116">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="585c9-116">isAzureAadRegistered</span></span>|<span data-ttu-id="585c9-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="585c9-117">Boolean</span></span>|<span data-ttu-id="585c9-118">True se o host registrado com o Windows Azure Active Directory dispositivo registro (BYOD dispositivos - ou seja, não totalmente gerenciados pelo enterprise).</span><span class="sxs-lookup"><span data-stu-id="585c9-118">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="585c9-119">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="585c9-119">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="585c9-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="585c9-120">Boolean</span></span>|<span data-ttu-id="585c9-121">True se o host é associado a um domínio do Active Directory no local de domínio.</span><span class="sxs-lookup"><span data-stu-id="585c9-121">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="585c9-122">Nome_netbios</span><span class="sxs-lookup"><span data-stu-id="585c9-122">netBiosName</span></span>|<span data-ttu-id="585c9-123">String</span><span class="sxs-lookup"><span data-stu-id="585c9-123">String</span></span>|<span data-ttu-id="585c9-124">O nome de host local, sem o nome de domínio DNS.</span><span class="sxs-lookup"><span data-stu-id="585c9-124">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="585c9-125">I-5.</span><span class="sxs-lookup"><span data-stu-id="585c9-125">os</span></span>|<span data-ttu-id="585c9-126">String</span><span class="sxs-lookup"><span data-stu-id="585c9-126">String</span></span>|<span data-ttu-id="585c9-127">Sistema operacional do host.</span><span class="sxs-lookup"><span data-stu-id="585c9-127">Host Operating System.</span></span> <span data-ttu-id="585c9-128">(Por exemplo, Windows10, MacOS, RHEL, etc.).</span><span class="sxs-lookup"><span data-stu-id="585c9-128">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="585c9-129">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="585c9-129">privateIpAddress</span></span>|<span data-ttu-id="585c9-130">String</span><span class="sxs-lookup"><span data-stu-id="585c9-130">String</span></span>|<span data-ttu-id="585c9-131">Endereço IPv4 ou IPv6 (não pode ser roteado) particular (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) no momento do alerta.</span><span class="sxs-lookup"><span data-stu-id="585c9-131">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="585c9-132">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="585c9-132">publicIpAddress</span></span>|<span data-ttu-id="585c9-133">String</span><span class="sxs-lookup"><span data-stu-id="585c9-133">String</span></span>|<span data-ttu-id="585c9-134">Endereço IPv4 ou IPv6 roteável publicamente (consulte [RFC 1918](https://tools.ietf.org/html/rfc1918)) em tempo de alerta.</span><span class="sxs-lookup"><span data-stu-id="585c9-134">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="585c9-135">riskScore</span><span class="sxs-lookup"><span data-stu-id="585c9-135">riskScore</span></span>|<span data-ttu-id="585c9-136">String</span><span class="sxs-lookup"><span data-stu-id="585c9-136">String</span></span>|<span data-ttu-id="585c9-137">Pontuação de risco de provedor-gerado/calculado do host.</span><span class="sxs-lookup"><span data-stu-id="585c9-137">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="585c9-138">Valor recomendado o intervalo de 0-1, que é igual a um percentual.</span><span class="sxs-lookup"><span data-stu-id="585c9-138">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="585c9-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="585c9-139">JSON representation</span></span>

<span data-ttu-id="585c9-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="585c9-140">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/hostsecuritystate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
