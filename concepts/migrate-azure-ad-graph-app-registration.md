---
title: Revisar o registro de aplicativos, permissões e problemas de migração de consentimento
description: Descreve o registro de aplicativo, permissão e migração de consentimento do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 06eeb5adeb1625559ca838a04590d2db65a03f97
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470645"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="57e11-103">Revisar o registro, permissões e consentimento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="57e11-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="57e11-104">Este artigo faz parte da *etapa 3:* revisar detalhes do aplicativo do [processo para migrar aplicativos.](migrate-azure-ad-graph-planning-checklist.md)</span><span class="sxs-lookup"><span data-stu-id="57e11-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="57e11-105">Para qualquer atualização de aplicativo, há três áreas a considerar:</span><span class="sxs-lookup"><span data-stu-id="57e11-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="57e11-106">**Registro de** aplicativo : você pode continuar a usar seu registro de aplicativo existente ( `appId` ) no código do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="57e11-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="57e11-107">Você não **precisa** registrar seu aplicativo para migrar para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57e11-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="57e11-108">Basta atualizar o código, testar fortemente e implantar a atualização.</span><span class="sxs-lookup"><span data-stu-id="57e11-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="57e11-109">**Permissões**: Você deve alterar suas permissões configuradas para as permissões equivalentes do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57e11-109">**Permissions**: You should change your configured permissions to the equivalent Microsoft Graph permissions.</span></span> <span data-ttu-id="57e11-110">Permissões delegadas concedidas para o Azure AD Graph também serão consideradas implicitamente concedidas para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57e11-110">Delegated permissions which were granted for Azure AD Graph will be implicitly considered granted for Microsoft Graph also.</span></span> <span data-ttu-id="57e11-111">Permissões de aplicativo (funções de aplicativo) precisarão ser concedidas novamente.</span><span class="sxs-lookup"><span data-stu-id="57e11-111">Application permissions (app roles) will need to be granted again.</span></span>

    <span data-ttu-id="57e11-112">Se sua atualização também inscui o uso de recursos ou recursos que não estão disponíveis para o Azure AD Graph, você provavelmente precisará solicitar permissões para esses novos recursos.</span><span class="sxs-lookup"><span data-stu-id="57e11-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="57e11-113">Se esse for o caso, você pode alternar seu aplicativo para usar o MSAL e o ponto de extremidade v2 e solicitar o consentimento adicional/incremental dinamicamente.</span><span class="sxs-lookup"><span data-stu-id="57e11-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="57e11-114">Encontre mais detalhes sobre como alternar para o MSAL em revisar alterações na biblioteca [de autenticação de aplicativos.](./migrate-azure-ad-graph-authentication-library.md)</span><span class="sxs-lookup"><span data-stu-id="57e11-114">Find more details about switching to MSAL in [review app authentication library changes](./migrate-azure-ad-graph-authentication-library.md).</span></span>

- <span data-ttu-id="57e11-115">**Consentimento**: Os usuários finais que já concederam consentimento para permissões delegadas (ou para quem o consentimento já foi concedido por um administrador) podem continuar usando seu aplicativo sem ser solicitado a conceder consentimento novamente.</span><span class="sxs-lookup"><span data-stu-id="57e11-115">**Consent**: End-users who have already granted consent for delegated permissions (or for whom consent has already been granted by an admin) can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="57e11-116">Os usuários que já concederam consentimento ao seu aplicativo para acessar seus dados podem continuar a usar seu aplicativo depois que ele tiver sido atualizado para usar o Microsoft Graph, sem que seja solicitado a consentir novamente.</span><span class="sxs-lookup"><span data-stu-id="57e11-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span> <span data-ttu-id="57e11-117">Novos usuários serão solicitados a consentir.</span><span class="sxs-lookup"><span data-stu-id="57e11-117">New users will be prompted for consent.</span></span>

<span data-ttu-id="57e11-118">Projetos de migração simples não devem ter problemas nessas áreas.</span><span class="sxs-lookup"><span data-stu-id="57e11-118">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="57e11-119">No entanto, se você usar novos recursos, serviços ou adicionar recursos adicionais, poderá precisar de novas permissões e o consentimento do usuário final pode ser necessário.</span><span class="sxs-lookup"><span data-stu-id="57e11-119">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="57e11-120">Nesses casos, o consentimento é solicitado quando os tokens são atualizados.</span><span class="sxs-lookup"><span data-stu-id="57e11-120">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="57e11-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="57e11-121">Next Steps</span></span>

- <span data-ttu-id="57e11-122">Saiba [as diferenças de biblioteca](migrate-azure-ad-graph-authentication-library.md) de autenticação entre o Azure AD Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="57e11-122">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="57e11-123">Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.</span><span class="sxs-lookup"><span data-stu-id="57e11-123">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>
