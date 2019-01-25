---
title: Use a API do Microsoft Graph para detecção de ameaças de segurança e proteção (preview)
description: A sofisticação das ameaças à segurança continua escalar, afetar a economia global. Dano quase sempre é feito muito antes de organizações mesmo descobrem a ele. Você pode usar o Microsoft Graph para criar ou estender as soluções de segurança que consolidem e correlacionam os alertas de segurança de várias fontes, detectarem ameaças que tentam comprometer a identidade do usuário, unlock dados contextuais para informar investigações e automatizar operações de segurança para maior eficiência.
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 37e98203e8f031aa98b35d82110a69e434c22a3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529926"
---
# <a name="use-the-microsoft-graph-api-for-security-threat-detection-and-protection-preview"></a><span data-ttu-id="ebf9e-105">Use a API do Microsoft Graph para detecção de ameaças de segurança e proteção (preview)</span><span class="sxs-lookup"><span data-stu-id="ebf9e-105">Use the Microsoft Graph API for security threat detection and protection (preview)</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebf9e-106">A sofisticação das ameaças à segurança continua escalar, afetar a economia global.</span><span class="sxs-lookup"><span data-stu-id="ebf9e-106">The sophistication of security threats continues to escalate, affecting the global economy.</span></span> <span data-ttu-id="ebf9e-107">Dano quase sempre é feito muito antes de organizações mesmo descobrem a ele.</span><span class="sxs-lookup"><span data-stu-id="ebf9e-107">Damage is often done long before organizations even discover it.</span></span> <span data-ttu-id="ebf9e-108">Você pode usar o Microsoft Graph para criar ou estender as soluções de segurança que consolidem e correlacionam os alertas de segurança de várias fontes, detectarem ameaças que tentam comprometer a identidade do usuário, unlock dados contextuais para informar investigações e automatizar operações de segurança para maior eficiência.</span><span class="sxs-lookup"><span data-stu-id="ebf9e-108">You can use Microsoft Graph to build or extend security solutions that consolidate and correlate security alerts from multiple sources, detect threats that attempt to compromise user identity, unlock contextual data to inform investigations, and automate security operations for greater efficiency.</span></span>

<span data-ttu-id="ebf9e-109">Gráfico de segurança inteligente reúne inteligência de segurança de dentro da Microsoft, centros de operações de segurança e parceiros de todo o mundo para formar um ecossistema de soluções integradas de segurança.</span><span class="sxs-lookup"><span data-stu-id="ebf9e-109">Intelligent Security Graph brings together security intelligence from within Microsoft, security operations centers, and partners from around the world to form an ecosystem of integrated security solutions.</span></span> <span data-ttu-id="ebf9e-110">Usando o aprendizado de máquina, o comportamento de monitoramento e a escala de nuvem, o gráfico de segurança inteligente pode melhor proteger, detectar e responder a ameaças de modo rápido e modo abrangente.</span><span class="sxs-lookup"><span data-stu-id="ebf9e-110">Using machine learning, behavioral monitoring, and the scale of the cloud, the Intelligent Security Graph can better protect, detect, and respond to threats quickly and comprehensively.</span></span> <span data-ttu-id="ebf9e-111">A [API de segurança](security-api-overview.md) , você se conecta ao [Gráfico de segurança inteligente](https://www.microsoft.com/en-us/security/intelligence-security-api), dando a você soluções que são acionáveis e abrangente.</span><span class="sxs-lookup"><span data-stu-id="ebf9e-111">The [security API](security-api-overview.md) connects you to the [Intelligent Security Graph](https://www.microsoft.com/en-us/security/intelligence-security-api), empowering you with solutions that are actionable and holistic.</span></span>

<span data-ttu-id="ebf9e-112">Os [eventos de risco de proteção de identidade API](identityprotection-root.md) oferece acesso fácil para os clientes do Windows Azure AD Premium P1 e P2 [detecções de risco feitas por proteção de identidade](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) de consulta e usar esses eventos em sistemas SIEM e aplicativos de segurança.</span><span class="sxs-lookup"><span data-stu-id="ebf9e-112">The [identity protection risk events API](identityprotection-root.md) gives easy access for Azure AD Premium P1 and P2 customers to query [risk detections made by Identity Protection](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-identityprotection-graph-getting-started) and use those events in SIEM systems and security applications.</span></span>

## <a name="see-also"></a><span data-ttu-id="ebf9e-113">Confira também</span><span class="sxs-lookup"><span data-stu-id="ebf9e-113">See also</span></span>

- [<span data-ttu-id="ebf9e-114">Por que usar a API de segurança?</span><span class="sxs-lookup"><span data-stu-id="ebf9e-114">Why use the security API?</span></span>](/graph/security-concept-overview#why-use-the-security-api-and-connect-with-microsoft-intelligent-security-graph)
- [<span data-ttu-id="ebf9e-115">Usar a API de segurança para integrar com gráfico de segurança inteligente</span><span class="sxs-lookup"><span data-stu-id="ebf9e-115">Use the security API to integrate with Intelligent Security Graph</span></span>](security-api-overview.md)
- <span data-ttu-id="ebf9e-116">Por que usar o Azure AD para proteger identidades em sua organização?</span><span class="sxs-lookup"><span data-stu-id="ebf9e-116">[Why use Azure AD to protect identities in your organization?](/graph/security-concept-overview#why-use-azure-ad-to-protect-identities-in-your-organization)</span></span>
- [<span data-ttu-id="ebf9e-117">Usar a API do Azure AD Identity Protection</span><span class="sxs-lookup"><span data-stu-id="ebf9e-117">Use the Azure AD Identity Protection API</span></span>](identityprotection-root.md)
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/security-reference-overview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
