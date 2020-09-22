---
title: Usar as APIs de proteção de identidade do Azure AD
description: Você pode usar o Microsoft Graph para consultar as APIs de proteção de identidade para receber informações sobre o risco detectado pela proteção de identidade do Azure AD.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 3da156079e6201ac73690c550bd56b246e30c870
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013556"
---
# <a name="use-the-azure-ad-identity-protection-api"></a><span data-ttu-id="1ed17-103">Usar a API de proteção de identidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="1ed17-103">Use the Azure AD identity protection API</span></span>

<span data-ttu-id="1ed17-104">Namespace: Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1ed17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ed17-105">A proteção de identidade é uma ferramenta que permite às organizações detectar, investigar e corrigir riscos baseados em identidade em seu ambiente.</span><span class="sxs-lookup"><span data-stu-id="1ed17-105">Identity Protection is a tool that allows organizations to discover, investigate, and remediate identity-based risks in their environment.</span></span> <span data-ttu-id="1ed17-106">Você pode usar as seguintes APIs do Microsoft Graph para consultar os riscos detectados pela proteção de identidade:</span><span class="sxs-lookup"><span data-stu-id="1ed17-106">You can use the following Microsoft Graph APIs to query risks detected by Identity Protection:</span></span> 

* <span data-ttu-id="1ed17-107">[riskDetection](riskdetection.md) -consulta o Microsoft Graph para obter uma lista de detecções de riscos vinculados de usuário e de entrada e informações associadas sobre a detecção.</span><span class="sxs-lookup"><span data-stu-id="1ed17-107">[riskDetection](riskdetection.md) - Query Microsoft Graph for a list of both user and sign-in linked risk detections and associated information about the detection.</span></span> <span data-ttu-id="1ed17-108">As detecções de risco na proteção de identidade do Azure AD incluem qualquer ação suspeita identificada relacionada às contas de usuário no diretório.</span><span class="sxs-lookup"><span data-stu-id="1ed17-108">Risk detections in Azure AD Identity Protection include any identified suspicious actions related to user accounts in the directory.</span></span>

* <span data-ttu-id="1ed17-109">[riskyUsers](riskyuser.md) – consulta o Microsoft Graph para obter informações sobre os usuários que a proteção de identidade detectou como arriscado.</span><span class="sxs-lookup"><span data-stu-id="1ed17-109">[riskyUsers](riskyuser.md) - Query Microsoft Graph for information about users that Identity Protection detected as risky.</span></span> <span data-ttu-id="1ed17-110">O risco do usuário representa a probabilidade de que uma determinada identidade ou conta seja comprometida.</span><span class="sxs-lookup"><span data-stu-id="1ed17-110">User risk represents the probability that a given identity or account is compromised.</span></span> <span data-ttu-id="1ed17-111">Esses riscos são calculados offline usando fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de imposição de leis, equipes de segurança da Microsoft e outras fontes confiáveis.</span><span class="sxs-lookup"><span data-stu-id="1ed17-111">These risks are calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="1ed17-112">[Sign](signin.md) -in – consultar o Microsoft Graph para obter informações sobre as entradas do Azure AD com propriedades específicas relacionadas ao estado, detalhes e nível do risco.</span><span class="sxs-lookup"><span data-stu-id="1ed17-112">[signIn](signin.md) - Query Microsoft Graph for information about Azure AD sign-ins with specific properties related to risk state, detail, and level.</span></span> <span data-ttu-id="1ed17-113">Um risco de entrada representa a probabilidade de que uma determinada solicitação de autenticação não seja autorizada pelo proprietário da identidade.</span><span class="sxs-lookup"><span data-stu-id="1ed17-113">A sign-in risk represents the probability that a given authentication request isn’t authorized by the identity owner.</span></span> <span data-ttu-id="1ed17-114">Esses riscos podem ser calculados em tempo real ou calculados offline usando fontes de inteligência de ameaças internas e externas da Microsoft, incluindo pesquisadores de segurança, profissionais de imposição de leis, equipes de segurança da Microsoft e outras fontes confiáveis.</span><span class="sxs-lookup"><span data-stu-id="1ed17-114">These risks can be calculated in real-time or calculated offline using Microsoft’s internal and external threat intelligence sources, including security researchers, law enforcement professionals, security teams at Microsoft, and other trusted sources.</span></span>

* <span data-ttu-id="1ed17-115">[identityRiskEvents](identityriskevent.md) – consulta o Microsoft Graph para obter uma lista de detecções de risco e informações associadas.</span><span class="sxs-lookup"><span data-stu-id="1ed17-115">[identityRiskEvents](identityriskevent.md) - Query Microsoft Graph for a list of risk detections and associated information.</span></span> <span data-ttu-id="1ed17-116">Essa API foi preterida; Recomendamos que você use **riskDetections** em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1ed17-116">This API is deprecated; we recommend that you use **riskDetections** instead.</span></span>

>[!CAUTION]
><span data-ttu-id="1ed17-117">A API **identityRiskEvents** foi preterida e interromperá o retorno de dados em 10 de janeiro de 2020.</span><span class="sxs-lookup"><span data-stu-id="1ed17-117">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="1ed17-118">Para obter detalhes, consulte [Preterition of the IDENTITYRISKEVENTS API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="1ed17-118">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

## <a name="see-also"></a><span data-ttu-id="1ed17-119">Confira também</span><span class="sxs-lookup"><span data-stu-id="1ed17-119">See also</span></span>

* [<span data-ttu-id="1ed17-120">Sobre a proteção de identidade do Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1ed17-120">About Azure Active Directory Identity Protection</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/overview-identity-protection)
* [<span data-ttu-id="1ed17-121">Introdução à proteção de identidade do Azure Active Directory e ao Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1ed17-121">Get started with Azure Active Directory identity protection and Microsoft Graph</span></span>](https://docs.microsoft.com/azure/active-directory/identity-protection/howto-identity-protection-graph-api)


