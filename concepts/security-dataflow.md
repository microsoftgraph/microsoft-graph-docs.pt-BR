---
title: Fluxo de dados da API de Segurança do Microsoft Graph
description: A API de Segurança do Microsoft Graph faz a federação de solicitações para todos os provedores no ecossistema de Segurança do Microsoft Graph. Isso tem base no consentimento do provedor de segurança fornecido pelo aplicativo, conforme mostrado no diagrama a seguir. O fluxo de trabalho de consentimento só se aplica a fornecedores diferentes da Microsoft.
author: Preetikr
ms.openlocfilehash: 5e70414409a35cc7fdef6fb85e6454e26a79bd38
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354737"
---
# <a name="microsoft-graph-security-api-data-flow"></a><span data-ttu-id="5f3a1-105">Fluxo de dados da API de Segurança do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="5f3a1-105">Microsoft Graph Security API data flow</span></span>

<span data-ttu-id="5f3a1-106">A API de Segurança do Microsoft Graph faz a federação de solicitações para todos os provedores no ecossistema de Segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-106">The Microsoft Graph Security API federates requests to all providers in the Microsoft Graph Security ecosystem.</span></span> <span data-ttu-id="5f3a1-107">Isso tem base no consentimento do provedor de segurança fornecido pelo aplicativo, conforme mostrado no diagrama a seguir.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-107">This is based on the security provider consent provided by the application, as shown in the following diagram.</span></span> <span data-ttu-id="5f3a1-108">O fluxo de trabalho de consentimento só se aplica a fornecedores diferentes da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-108">The consent workflow only applies to non-Microsoft providers.</span></span>

![security_dataflow_1.png](./images/security-dataflow-1.png)

<span data-ttu-id="5f3a1-110">Veja a seguir uma descrição do fluxo:</span><span class="sxs-lookup"><span data-stu-id="5f3a1-110">The following is a description of the flow:</span></span>

1. <span data-ttu-id="5f3a1-111">O usuário do aplicativo entra no aplicativo provedor para exibir o formulário de consentimento do provedor.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-111">The application user signs in to the provider application to view the consent form from the provider.</span></span> <span data-ttu-id="5f3a1-112">Essa experiência, ou interface do usuário, de formulário de consentimento pertence ao provedor e se aplica apenas a fornecedores diferentes da Microsoft, a fim de obter o consentimento explícito de seus clientes para enviar as solicitações à API de Segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-112">This consent form experience or UI is owned by the provider and applies to non-Microsoft providers only to get explicit consent from their customers to send requests to Microsoft Graph Security API.</span></span>
2. <span data-ttu-id="5f3a1-113">O consentimento do cliente é armazenado no lado do provedor.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-113">The client consent is stored on the provider side.</span></span>
3. <span data-ttu-id="5f3a1-114">O serviço de consentimento do provedor chama a API de Segurança do Microsoft Graph para informar a aprovação de consentimento para o cliente respectivo.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-114">The provider consent service calls the Microsoft Graph Security API to inform consent approval for the respective customer.</span></span>
4. <span data-ttu-id="5f3a1-115">O aplicativo envia uma solicitação à API de Segurança do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-115">The application sends a request to the Microsoft Graph Security API.</span></span>
5. <span data-ttu-id="5f3a1-116">A API de Segurança do Microsoft Graph verifica as informações de consentimento para esse cliente mapeado para vários provedores.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-116">The Microsoft Graph Security API checks for the consent information for this customer mapped to various providers.</span></span>
6. <span data-ttu-id="5f3a1-117">A API de Segurança do Microsoft Graph chama todos os provedores aos quais o cliente concedeu consentimento explícito por meio da experiência de consentimento do provedor.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-117">The Microsoft Graph Security API calls all those providers the customer has given explicit consent to via the provider consent experience.</span></span>
7. <span data-ttu-id="5f3a1-118">A resposta é devolvida por todos os provedores com consentimento para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-118">The response is returned from all the consented providers for that client.</span></span>
8. <span data-ttu-id="5f3a1-119">A resposta com o conjunto de resultados retorna para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-119">The result set response is returned to the application.</span></span>
9. <span data-ttu-id="5f3a1-120">Se o cliente não tiver dado o consentimento a qualquer provedor, nenhum resultado desses provedores será incluído na resposta.</span><span class="sxs-lookup"><span data-stu-id="5f3a1-120">If the customer has not consented to any provider, no results from those providers are included in the response.</span></span>
