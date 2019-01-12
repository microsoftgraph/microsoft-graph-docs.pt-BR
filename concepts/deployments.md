---
title: Implantações de nuvens nacionais
description: Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas. Essas versões de nuvem nacional são instâncias isoladas de redes físicas e lógicas dos serviços de nuvem corporativa da Microsoft, que são confinados pelas fronteiras geográficas de países específicos e operados pela equipe local. Para saber mais, confira Nuvens nacionais da Microsoft.
localization_priority: Priority
ms.openlocfilehash: b22fce675bc97d0f22833d89dab01afd18e06032
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840415"
---
# <a name="national-cloud-deployments"></a><span data-ttu-id="e8110-105">Implantações de nuvem nacional</span><span class="sxs-lookup"><span data-stu-id="e8110-105">National cloud deployments</span></span>


<span data-ttu-id="e8110-106">Além de uma rede global de datacenters, os serviços em nuvem da Microsoft estão disponíveis em três nuvens nacionais separadas.</span><span class="sxs-lookup"><span data-stu-id="e8110-106">In addition to our global network of datacenters, Microsoft cloud services are available in three separate national clouds.</span></span> <span data-ttu-id="e8110-107">Essas versões de nuvens nacionais são instâncias isoladas de redes físicas e lógicas dos serviços de nuvem corporativa da Microsoft, que são confinados pelas fronteiras geográficas de países específicos e operados pela equipe local.</span><span class="sxs-lookup"><span data-stu-id="e8110-107">These national cloud versions are physical and logical network-isolated instances of Microsoft enterprise cloud services, which are confined within the geographic borders of specific countries and operated by local personnel.</span></span> <span data-ttu-id="e8110-108">Para saber mais, confira [Nuvens nacionais da Microsoft](https://www.microsoft.com/pt-BR/TrustCenter/CloudServices/NationalCloud).</span><span class="sxs-lookup"><span data-stu-id="e8110-108">To learn more, see [Microsoft National Clouds](https://www.microsoft.com/pt-BR/TrustCenter/CloudServices/NationalCloud).</span></span>

<span data-ttu-id="e8110-109">As nuvens nacionais atuais incluem:</span><span class="sxs-lookup"><span data-stu-id="e8110-109">Current national clouds include:</span></span>

- <span data-ttu-id="e8110-110">Microsoft Cloud para o Governo dos EUA</span><span class="sxs-lookup"><span data-stu-id="e8110-110">Microsoft Cloud for US Government</span></span>
- <span data-ttu-id="e8110-111">Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="e8110-111">Microsoft Cloud Germany</span></span>
- <span data-ttu-id="e8110-112">Azure e Office 365 operados pela 21Vianet na China</span><span class="sxs-lookup"><span data-stu-id="e8110-112">Azure and Office 365 operated by 21Vianet in China</span></span>

<span data-ttu-id="e8110-113">Este artigo fornece informações sobre as diferentes implantações de nuvem nacional do Microsoft Graph e os recursos em cada implantação que estão disponíveis para os desenvolvedores.</span><span class="sxs-lookup"><span data-stu-id="e8110-113">This article provides information about the different national cloud deployments of Microsoft Graph and the capabilities within each deployment that are available to developers.</span></span>

## <a name="microsoft-graph-and-microsoft-graph-explorer-service-root-endpoints"></a><span data-ttu-id="e8110-114">Pontos de extremidade raiz de serviço do Microsoft Graph e do Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="e8110-114">Microsoft Graph and Microsoft Graph Explorer service root endpoints</span></span>

<span data-ttu-id="e8110-115">A tabela a seguir mostra os pontos de extremidade do serviço raiz do Microsoft Graph e o Microsoft Graph Explorer para cada nuvem nacional.</span><span class="sxs-lookup"><span data-stu-id="e8110-115">The following table shows the service root endpoints for Microsoft Graph and Microsoft Graph Explorer for each National cloud.</span></span>

| <span data-ttu-id="e8110-116">National Cloud</span><span class="sxs-lookup"><span data-stu-id="e8110-116">National Cloud</span></span> | <span data-ttu-id="e8110-117">Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e8110-117">Microsoft Graph</span></span> | <span data-ttu-id="e8110-118">Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="e8110-118">Microsoft Graph Explorer</span></span>
|---------------------------|----------------|----------------|
| <span data-ttu-id="e8110-119">Microsoft Graph China operado pela 21Vianet</span><span class="sxs-lookup"><span data-stu-id="e8110-119">Microsoft Graph China operated by 21Vianet</span></span> | https://microsoftgraph.chinacloudapi.cn | https://developer.microsoft.com/zh-cn/graph/graph-explorer-china |
| <span data-ttu-id="e8110-120">Microsoft Graph Alemanha</span><span class="sxs-lookup"><span data-stu-id="e8110-120">Microsoft Graph Germany</span></span> | https://graph.microsoft.de | <span data-ttu-id="e8110-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8110-121">Not supported.</span></span> |
| <span data-ttu-id="e8110-122">Microsoft Graph para o Governo dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="e8110-122">Microsoft Graph for US Government</span></span> | https://graph.microsoft.com | <span data-ttu-id="e8110-123">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8110-123">Not supported.</span></span> |
| <span data-ttu-id="e8110-124">Serviço global do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e8110-124">Microsoft Graph global service</span></span> | https://graph.microsoft.com | https://developer.microsoft.com/graph/graph-explorer |

> <span data-ttu-id="e8110-125">**Nota**: os aplicativos só podem acessar dados organizacionais por meio de pontos de extremidade de nuvens nacionais.</span><span class="sxs-lookup"><span data-stu-id="e8110-125">**Note**: Apps can only access organizational data through the national cloud endpoints.</span></span> <span data-ttu-id="e8110-126">Isso significa que somente os dados em locatários registrados na nuvem nacional específica podem ser acessados.</span><span class="sxs-lookup"><span data-stu-id="e8110-126">This means that only data in tenants registered in the specific national cloud can be accessed.</span></span> <span data-ttu-id="e8110-127">Os aplicativos que estão tentando acessar dados de consumidor associados a uma conta Microsoft pessoal através do Microsoft Graph devem usar o serviço global https://graph.microsoft.com).</span><span class="sxs-lookup"><span data-stu-id="e8110-127">Apps that are trying to access consumer data associated with personal Microsoft accounts through Microsoft Graph should use the global service (https://graph.microsoft.com).</span></span> <span data-ttu-id="e8110-128">Os tokens de acesso adquiridos para uma implantação de nuvens nacionais não são intercambiáveis com aqueles adquiridos para o serviço global.</span><span class="sxs-lookup"><span data-stu-id="e8110-128">Access tokens acquired for a national cloud deployment are not interchangeable with those acquired for the global service.</span></span>

## <a name="azure-ad-openid-connect-and-oauth20-endpoints"></a><span data-ttu-id="e8110-129">Pontos de extremidade Azure AD OpenID Connect e OAuth2.0</span><span class="sxs-lookup"><span data-stu-id="e8110-129">Azure AD OpenID Connect and OAuth2.0 endpoints</span></span>

<span data-ttu-id="e8110-130">A tabela a seguir lista as URLs base para os pontos de extremidade do Azure AD (Azure Active Directory) usados para adquirir tokens para chamar o Microsoft Graph para cada nuvem nacional.</span><span class="sxs-lookup"><span data-stu-id="e8110-130">The following table lists the base URLs for the Azure Active Directory (Azure AD) endpoints used to acquire tokens to call Microsoft Graph for each national cloud.</span></span>

| <span data-ttu-id="e8110-131">National Cloud</span><span class="sxs-lookup"><span data-stu-id="e8110-131">National Cloud</span></span> | <span data-ttu-id="e8110-132">Ponto de extremidade do Microsoft Azure AD raiz</span><span class="sxs-lookup"><span data-stu-id="e8110-132">Azure AD root endpoint</span></span> |
|---------------------------|----------------|
| <span data-ttu-id="e8110-133">Microsoft Azure AD China operado pela 21Vianet</span><span class="sxs-lookup"><span data-stu-id="e8110-133">Azure AD China operated by 21Vianet</span></span> |https://login.chinacloudapi.cn |
| <span data-ttu-id="e8110-134">Microsoft Azure AD Alemanha</span><span class="sxs-lookup"><span data-stu-id="e8110-134">Azure AD Germany</span></span> | https://login.microsoftonline.de |
| <span data-ttu-id="e8110-135">Microsoft Azure AD para o Governo dos Estados Unidos</span><span class="sxs-lookup"><span data-stu-id="e8110-135">Azure AD for US Government</span></span> | https://login.microsoftonline.us |
| <span data-ttu-id="e8110-136">Microsoft Azure AD (serviço global)</span><span class="sxs-lookup"><span data-stu-id="e8110-136">Azure AD (global service)</span></span> | https://login.microsoftonline.com |

<span data-ttu-id="e8110-p104">As solicitações para autorização do Microsoft Azure AD ou dos pontos de extremidades de tokens podem ser formadas usando a URL de base específica da região apropriada. Por exemplo, para a Alemanha:</span><span class="sxs-lookup"><span data-stu-id="e8110-p104">Requests to the Azure AD authorization or token endpoints can be formed using the appropriate region-specific base URL. For example, for Germany:</span></span>

- <span data-ttu-id="e8110-139">O ponto de extremidade comum para autorização é https://login.microsoftonline.de/common/oauth2/authorize.</span><span class="sxs-lookup"><span data-stu-id="e8110-139">The authorization common endpoint is https://login.microsoftonline.de/common/oauth2/authorize.</span></span>
- <span data-ttu-id="e8110-140">O ponto de extremidade comum para token é https://login.microsoftonline.de/common/oauth2/token.</span><span class="sxs-lookup"><span data-stu-id="e8110-140">The token common endpoint is https://login.microsoftonline.de/common/oauth2/token.</span></span>

<span data-ttu-id="e8110-p105">Pontos de extremidade específicos do locatário podem ser formados por meio da substituição de "comum" nas URLs acima pela ID de locatário ou um domínio verificado para o locatário. O uso de pontos de extremidade comuns ou específicos do locatário dependerá dos requisitos do aplicativo e do fluxo de autenticação que você está usando para obter tokens. Para saber mais sobre tokens de acesso do Azure AD e do Microsoft Graph, confira [Obter tokens de autenticação](./auth-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e8110-p105">Tenant-specific endpoints can be formed by replacing "common" in the URLs above with either the tenant ID or a verified domain for the tenant. Whether you use the common or tenant-specific endpoints will depend upon the requirements of your app and the authentication flow you are using to get tokens. To learn more about Azure AD access tokens and Microsoft Graph, see [Get auth tokens](./auth-overview.md).</span></span>

> <span data-ttu-id="e8110-144">**Observação:** Os [pontos de extremidade de Azure autorização e token do AD v 2.0](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-appmodel-v2-overview/) estão disponíveis apenas no serviço global. Eles ainda não têm suporte para uso com implantações de nuvem nacional.</span><span class="sxs-lookup"><span data-stu-id="e8110-144">**Note:** The [Azure AD v2.0 authorization and token endpoints](https://azure.microsoft.com/pt-BR/documentation/articles/active-directory-appmodel-v2-overview/) are available on the global service only; they are not yet supported for use with national cloud deployments.</span></span>

## <a name="supported-features"></a><span data-ttu-id="e8110-145">Recursos com suporte</span><span class="sxs-lookup"><span data-stu-id="e8110-145">Supported features</span></span>

<span data-ttu-id="e8110-146">Os seguintes recursos do Microsoft Graph estão geralmente disponíveis (no ponto de extremidade `/v1.0`) em todas as implantações de nuvens nacionais, exceto quando indicado:</span><span class="sxs-lookup"><span data-stu-id="e8110-146">The following Microsoft Graph features are generally available (on the `/v1.0` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="e8110-147">Usuários</span><span class="sxs-lookup"><span data-stu-id="e8110-147">Users</span></span>
* <span data-ttu-id="e8110-148">Grupos</span><span class="sxs-lookup"><span data-stu-id="e8110-148">Groups</span></span>
* <span data-ttu-id="e8110-149">Excel (o suporte é limitado no Microsoft Graph operado pela 21Vianet na China.)</span><span class="sxs-lookup"><span data-stu-id="e8110-149">Excel (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e8110-150">OneDrive (o suporte é limitado no Microsoft Graph operado pela 21Vianet na China.)</span><span class="sxs-lookup"><span data-stu-id="e8110-150">OneDrive (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e8110-151">Email do Outlook</span><span class="sxs-lookup"><span data-stu-id="e8110-151">Outlook Mail</span></span>
* <span data-ttu-id="e8110-152">Calendário do Outlook</span><span class="sxs-lookup"><span data-stu-id="e8110-152">Outlook Calendar</span></span>
* <span data-ttu-id="e8110-153">Contatos Pessoais</span><span class="sxs-lookup"><span data-stu-id="e8110-153">Personal Contacts</span></span> 
* <span data-ttu-id="e8110-154">SharePoint (o suporte é limitado no Microsoft Graph operado pela 21Vianet na China.)</span><span class="sxs-lookup"><span data-stu-id="e8110-154">SharePoint (Support is limited on Microsoft Graph operated by 21Vianet in China.)</span></span>
* <span data-ttu-id="e8110-155">Consulta delta (o suporte varia entre diferentes recursos em cada implantação de nuvem nacional.)</span><span class="sxs-lookup"><span data-stu-id="e8110-155">Delta query (Support varies across different resources on each national cloud deployment.)</span></span>
* <span data-ttu-id="e8110-156">Webhooks (o suporte varia entre diferentes recursos em cada implantação de nuvem nacional.)</span><span class="sxs-lookup"><span data-stu-id="e8110-156">Webhooks (Support varies across different resources on each national cloud deployment.)</span></span>

<span data-ttu-id="e8110-157">Os seguintes recursos adicionais do Microsoft Graph estão disponíveis na visualização (no ponto de extremidade `/beta`) em todas as implantações de nuvens nacionais, exceto quando indicado:</span><span class="sxs-lookup"><span data-stu-id="e8110-157">The following addtional Microsoft Graph features are available in preview (on the `/beta` endpoint) across all national cloud deployments, except where noted:</span></span>

* <span data-ttu-id="e8110-158">Contatos organizacionais</span><span class="sxs-lookup"><span data-stu-id="e8110-158">Organizational Contacts</span></span>
* <span data-ttu-id="e8110-159">Aplicativos</span><span class="sxs-lookup"><span data-stu-id="e8110-159">Applications</span></span>
* <span data-ttu-id="e8110-160">Entidades de serviço</span><span class="sxs-lookup"><span data-stu-id="e8110-160">Service Principals</span></span>

<span data-ttu-id="e8110-161">Os seguintes recursos do Microsoft Graph ainda não têm suporte em implantações de nuvem nacionais:</span><span class="sxs-lookup"><span data-stu-id="e8110-161">The following Microsoft Graph features are not yet supported on national cloud deployments:</span></span>

* <span data-ttu-id="e8110-162">Microsoft Planner</span><span class="sxs-lookup"><span data-stu-id="e8110-162">Microsoft Planner</span></span>
* <span data-ttu-id="e8110-163">Extensões de esquema de diretório</span><span class="sxs-lookup"><span data-stu-id="e8110-163">Directory schema extensions</span></span>
* <span data-ttu-id="e8110-164">Extensões de tipo aberto</span><span class="sxs-lookup"><span data-stu-id="e8110-164">Open type extensions</span></span>
