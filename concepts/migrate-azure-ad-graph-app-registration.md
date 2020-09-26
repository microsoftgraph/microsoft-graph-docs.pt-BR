---
title: Revisar problemas de migração de registro, permissões e autorização de aplicativo
description: Descreve o registro de aplicativo, permissão e migração de consentimento do Azure Active Directory (Azure AD) para a API do Microsoft Graph.
author: dkershaw10
localization_priority: Normal
ms.prod: azure-active-directory
ms.openlocfilehash: 8cca43199d8549841087a84d1bd275e38f09efdb
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2020
ms.locfileid: "48288340"
---
# <a name="review-app-registration-permissions-and-consent"></a><span data-ttu-id="fb527-103">Revisar o registro, as permissões e o consentimento do aplicativo</span><span class="sxs-lookup"><span data-stu-id="fb527-103">Review app registration, permissions, and consent</span></span>

<span data-ttu-id="fb527-104">Este artigo faz parte da *etapa 3: revise os detalhes do aplicativo* do [processo para migrar aplicativos](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="fb527-104">This article is part of *step 3: review app details* of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="fb527-105">Para qualquer atualização de aplicativos, há três áreas que devem ser consideradas:</span><span class="sxs-lookup"><span data-stu-id="fb527-105">For any app update, there are three areas to consider:</span></span>

- <span data-ttu-id="fb527-106">**Registro do aplicativo**: você pode continuar a usar seu registro de aplicativo existente ( `appId` ) no seu código de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb527-106">**App registration**: You can continue to use your existing app registration (`appId`) in your application code.</span></span>  

    <span data-ttu-id="fb527-107">Você **não** precisa registrar seu aplicativo novamente para migrar para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb527-107">You do **not** have to re-register your app to migrate to Microsoft Graph.</span></span> <span data-ttu-id="fb527-108">Basta atualizar o código, testar fortemente e implantar sua atualização.</span><span class="sxs-lookup"><span data-stu-id="fb527-108">Simply update the code, test heavily, and then deploy your update.</span></span>  

- <span data-ttu-id="fb527-109">**Permissões**: você pode continuar a usar as permissões configuradas existentes para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="fb527-109">**Permissions**: You can continue to use the existing configured permissions for your app.</span></span> <span data-ttu-id="fb527-110">Você não precisa solicitar novas permissões porque as permissões do Azure AD Graph são compartilhadas com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb527-110">You do not have to request new permissions because Azure AD Graph permissions are shared with Microsoft Graph.</span></span>

    <span data-ttu-id="fb527-111">Por exemplo, se o aplicativo existente tiver as permissões _User. Read. All_ e _Group. Read. All_ , essas permissões também serão implicitamente concedidas ao seu aplicativo atualizado para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb527-111">For example, if your existing app has _User.Read.All_ and _Group.Read.All_ permissions, those permissions are implicitly granted to your updated app for Microsoft Graph as well.</span></span>

    <span data-ttu-id="fb527-112">Se sua atualização também Incudes o uso de recursos ou recursos que não estão disponíveis para o Azure AD Graph, provavelmente você precisará solicitar permissões para esses novos recursos.</span><span class="sxs-lookup"><span data-stu-id="fb527-112">If your update also incudes the use of features or capabilities that aren't available to Azure AD Graph, you'll likely need to request permissions for these new features.</span></span> <span data-ttu-id="fb527-113">Se esse for o caso, você pode mudar seu aplicativo para usar o MSAL e o ponto de extremidade V2 e solicitar o consentimento adicional/incremental dinamicamente.</span><span class="sxs-lookup"><span data-stu-id="fb527-113">If that's the case, you can switch your app to use MSAL and the v2 endpoint, and request additional/incremental consent dynamically.</span></span> <span data-ttu-id="fb527-114">Encontre mais detalhes sobre a mudança para o MSAL em [revisar alterações na biblioteca de autenticação de aplicativos](./migrate-azure-ad-graph-authentication-library.md).</span><span class="sxs-lookup"><span data-stu-id="fb527-114">Find more details about switching to MSAL in [review app authentication library changes](./migrate-azure-ad-graph-authentication-library.md).</span></span>

- <span data-ttu-id="fb527-115">**Consentimento**: os usuários finais podem continuar usando o aplicativo sem precisar conceder o consentimento novamente.</span><span class="sxs-lookup"><span data-stu-id="fb527-115">**Consent**: End-users can continue using your app without being asked to grant consent again.</span></span>

    <span data-ttu-id="fb527-116">Os usuários que já concederam o consentimento do seu aplicativo para acessar seus dados podem continuar a usar seu aplicativo após ele ter sido atualizado para usar o Microsoft Graph, sem solicitar o consentimento.</span><span class="sxs-lookup"><span data-stu-id="fb527-116">Users who have already granted consent to your app to access their data can continue to use your app after it's been updated to use Microsoft Graph, without being asked to consent again.</span></span>

<span data-ttu-id="fb527-117">Projetos de migração simples não devem ter problemas nessas áreas.</span><span class="sxs-lookup"><span data-stu-id="fb527-117">Simple migration projects should experience no issues in these areas.</span></span>

<span data-ttu-id="fb527-118">No entanto, se você usar novos recursos, serviços ou adicionar recursos adicionais, talvez precise de novas permissões e o consentimento do usuário final possa ser necessário.</span><span class="sxs-lookup"><span data-stu-id="fb527-118">However, if you use new features, services, or add additional capabilities, you may need new permissions and end-user consent may be required.</span></span>  <span data-ttu-id="fb527-119">Nesses casos, o consentimento é solicitado quando os tokens são atualizados.</span><span class="sxs-lookup"><span data-stu-id="fb527-119">In such cases, consent is requested when tokens are refreshed.</span></span>

## <a name="next-steps"></a><span data-ttu-id="fb527-120">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="fb527-120">Next Steps</span></span>

- <span data-ttu-id="fb527-121">Saiba mais sobre as diferenças da [biblioteca de autenticação](migrate-azure-ad-graph-authentication-library.md) entre o Azure ad Graph e o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="fb527-121">Learn [authentication library](migrate-azure-ad-graph-authentication-library.md) differences between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="fb527-122">Revise a [lista de verificação](migrate-azure-ad-graph-planning-checklist.md) novamente.</span><span class="sxs-lookup"><span data-stu-id="fb527-122">Review the [checklist](migrate-azure-ad-graph-planning-checklist.md) again.</span></span>