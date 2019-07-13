---
title: Implantar, testar e estender aplicativos migrados
description: 'Descreve como migrar aplicativos do Azure Active Directory (Azure AD) para usar a API do Microsoft Graph (REST); isso aborda a etapa 3: implantar, testar e estender.'
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6b5236f6b7be140e1040a3169edded6e162b5e7a
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645249"
---
# <a name="deploy-test-and-extend"></a><span data-ttu-id="d4757-103">Implantar, testar e estender</span><span class="sxs-lookup"><span data-stu-id="d4757-103">Deploy, test, and extend</span></span>

<span data-ttu-id="d4757-104">Esta é a etapa 4 do [processo de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="d4757-104">This is step 4 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

1.  <span data-ttu-id="d4757-105">**Teste por meio**</span><span class="sxs-lookup"><span data-stu-id="d4757-105">**Test throughly**</span></span>

    <span data-ttu-id="d4757-106">Depois de atualizar o aplicativo, teste-o cuidadosamente para verificar se ele funciona conforme o esperado e se você não introduziu nenhuma regressão.</span><span class="sxs-lookup"><span data-stu-id="d4757-106">Once you've updated your app, test it thoroughly to verify that it works as expected and that you haven't introduced any regressions.</span></span>  

    <span data-ttu-id="d4757-107">Certifique-se de usar vários ambientes, conjuntos de dados e pessoas de usuário final, por exemplo, credenciais com diferentes funções, direitos e responsabilidades.</span><span class="sxs-lookup"><span data-stu-id="d4757-107">Be sure to use multiple environments, data sets, and end-user personas, e.g. credentials with different roles, rights, and responsibilities.</span></span> <span data-ttu-id="d4757-108">Percorra todo o ciclo de vida, fazendo com que um novo usuário de teste adquira o aplicativo pela primeira vez, bem como um usuário existente (que já tenha remetido) tentando usar o aplicativo novamente.</span><span class="sxs-lookup"><span data-stu-id="d4757-108">Go through the entire lifecycle, by having a new test user acquire the app for the first time, as well as an existing user (who already consented) trying to use the app again.</span></span>

2.  <span data-ttu-id="d4757-109">**Implantar atualizações em estágios**</span><span class="sxs-lookup"><span data-stu-id="d4757-109">**Deploy staged updates**</span></span>

    <span data-ttu-id="d4757-110">Considere a implantação de suas atualizações em estágios.</span><span class="sxs-lookup"><span data-stu-id="d4757-110">Consider deploying your updates in stages.</span></span>  <span data-ttu-id="d4757-111">Uma distribuição limitada para um pequeno conjunto de usuários amigáveis pode ajudar a identificar falhas e outros problemas desagradáveis.</span><span class="sxs-lookup"><span data-stu-id="d4757-111">A limited roll-out to a small set of friendly users can help identify glitches and other potentially-embarrassing issues.</span></span>  <span data-ttu-id="d4757-112">Isso também lhe dá a oportunidade de monitorar a recepção inicial e os comentários.</span><span class="sxs-lookup"><span data-stu-id="d4757-112">This also gives you a chance to monitor initial reception and feedback.</span></span>

    <span data-ttu-id="d4757-113">Se a distribuição inicial ficar bem, monitore o progresso à medida que você implanta em grandes audiências.</span><span class="sxs-lookup"><span data-stu-id="d4757-113">If the initial roll-out goes well, monitor progress as you deploy to larger audiences.</span></span>

3.  <span data-ttu-id="d4757-114">**Explorar novo valor**</span><span class="sxs-lookup"><span data-stu-id="d4757-114">**Explore new value**</span></span>

    <span data-ttu-id="d4757-115">Agora você já fez a migração para o Microsoft Graph, nunca foi mais fácil desbloquear muito mais conjuntos de informações e recursos que agora estão em suas mãos.</span><span class="sxs-lookup"><span data-stu-id="d4757-115">Now you've made the switch to Microsoft Graph, it's never been easier for you to unlock many more datasets and features that are now at your fingertips.</span></span> <span data-ttu-id="d4757-116">Verifique se há novos conjuntos de recursos e capacidades regularmente.</span><span class="sxs-lookup"><span data-stu-id="d4757-116">Check for new datasets and capabilities regularly.</span></span>  

    - <span data-ttu-id="d4757-117">Dê uma olhada no [que você pode fazer com o Microsoft Graph](/graph/examples)</span><span class="sxs-lookup"><span data-stu-id="d4757-117">Take a look at [what you can do with Microsoft Graph](/graph/examples)</span></span>
    - <span data-ttu-id="d4757-118">Explore o [blog do Microsoft Graph](/graph/blogs) para obter as últimas notícias sobre o Microsoft Graph e algumas boas séries de aprendizado.</span><span class="sxs-lookup"><span data-stu-id="d4757-118">Explore the [Microsoft Graph blog](/graph/blogs) for the latest news about Microsoft Graph and some great learning series.</span></span>
    - <span data-ttu-id="d4757-119">O [changelog](/greaph/changelog) resume as atualizações de serviço e de documento.</span><span class="sxs-lookup"><span data-stu-id="d4757-119">The [changelog](/greaph/changelog) summarizes service and document updates.</span></span> <span data-ttu-id="d4757-120">Seguir essas atualizações o ajudará a rastrear novas APIs introduzidas no/beta (visualização) e aquelas promovidas para a versão v 1.0 (GA).</span><span class="sxs-lookup"><span data-stu-id="d4757-120">Following these updates will help you track new APIs introduced to /beta (preview) and those promoted to v1.0 (GA).</span></span>  <span data-ttu-id="d4757-121">Essas novas APIs podem fornecer novas maneiras de adicionar mais valor e novas experiências aos seus aplicativos.</span><span class="sxs-lookup"><span data-stu-id="d4757-121">These new APIs can provide new ways for you to add more value and new experiences to your apps.</span></span>  

## <a name="see-also"></a><span data-ttu-id="d4757-122">Confira também</span><span class="sxs-lookup"><span data-stu-id="d4757-122">See also</span></span>

<span data-ttu-id="d4757-123">Se você encontrar problemas ou precisar de ajuda durante o processo de migração, você pode:</span><span class="sxs-lookup"><span data-stu-id="d4757-123">If you run into problems or need help during the migration process, you can:</span></span>

- <span data-ttu-id="d4757-124">Revise a [lista de verificação](migrate-azure-ad-graph-overview.md) novamente</span><span class="sxs-lookup"><span data-stu-id="d4757-124">Review the [checklist](migrate-azure-ad-graph-overview.md) again</span></span>
- <span data-ttu-id="d4757-125">Postar perguntas no [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span><span class="sxs-lookup"><span data-stu-id="d4757-125">Post questions to [StackOverflow](https://stackoverflow.com/questions/tagged/microsoft-graph)</span></span>
- <span data-ttu-id="d4757-126">Revise as amostras do Microsoft Graph para comparar e comparar com o código do aplicativo existente:</span><span class="sxs-lookup"><span data-stu-id="d4757-126">Review Microsoft Graph samples to contrast and compare with your existing application code:</span></span>
  - <span data-ttu-id="d4757-127">**Aplicativos que usam a API REST**: explorar [inícios e amostras rápidas](https://developer.microsoft.com/graph/get-started), escolhendo sua plataforma de escolha e executar o início rápido ou pesquisar um exemplo apropriado</span><span class="sxs-lookup"><span data-stu-id="d4757-127">**Apps that use the REST API**: explore [quick starts and samples](https://developer.microsoft.com/graph/get-started), choosing your platform of choice and run through the quick start or search for an appropriate sample</span></span>
  - <span data-ttu-id="d4757-128">**Aplicativo que usa a biblioteca de cliente .net**: examinar [console-Csharp-Snippets-Sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) e/ou [dotnetcore-console-Sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span><span class="sxs-lookup"><span data-stu-id="d4757-128">**App that use the .NET client library**: review [console-csharp-snippets-sample](https://github.com/microsoftgraph/console-csharp-snippets-sample) and/or [dotnetcore-console-sample](https://github.com/microsoftgraph/dotnetcore-console-sample)</span></span>

## <a name="next-steps"></a><span data-ttu-id="d4757-129">Próximos passos</span><span class="sxs-lookup"><span data-stu-id="d4757-129">Next Steps</span></span>

- <span data-ttu-id="d4757-130">Use [inícios e amostras rápidas](/graph/get-started) para se familiarizar rapidamente.</span><span class="sxs-lookup"><span data-stu-id="d4757-130">Use [quick starts and samples](/graph/get-started) to come up to speed quickly.</span></span>
- <span data-ttu-id="d4757-131">Aproveitar [bibliotecas de clientes e SDKs](https://developer.microsoft.com/graph/get-started) para desenvolver aplicativos personalizados</span><span class="sxs-lookup"><span data-stu-id="d4757-131">Leverage [client libraries and SDKs](https://developer.microsoft.com/graph/get-started) to develop custom applications</span></span> 
- <span data-ttu-id="d4757-132">Explore os conceitos e as práticas [do Microsoft Graph](/graph/overview) .</span><span class="sxs-lookup"><span data-stu-id="d4757-132">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="d4757-133">Use o [Explorador do Graph](https://aka.ms/ge) para experimentar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d4757-133">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
