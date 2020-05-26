---
title: Referência da API REST do Microsoft Graph v1.0
description: Bem-vindo à referência da API REST do Microsoft Graph para o ponto de extremidade v1.0.
localization_priority: Priority
author: angelgolfer-ms
ms.prod: non-product-specific
doc_type: conceptualPageType
ms.openlocfilehash: 971cfc675fce4c4633c4e331ca20679321112ad8
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353424"
---
# <a name="microsoft-graph-rest-api-v10-reference"></a><span data-ttu-id="28d44-103">Referência da API REST do Microsoft Graph v1.0</span><span class="sxs-lookup"><span data-stu-id="28d44-103">Microsoft Graph REST API v1.0 reference</span></span>

<span data-ttu-id="28d44-104">Bem-vindo à referência da API REST do Microsoft Graph para o ponto de extremidade v1.0.</span><span class="sxs-lookup"><span data-stu-id="28d44-104">Welcome to Microsoft Graph REST API reference for the v1.0 endpoint.</span></span>

<span data-ttu-id="28d44-105">Os conjuntos de APIs no ponto de extremidade v1.0 (`https://graph.microsoft.com/v1.0`) estão no status de disponibilidade geral (GA) e passaram por um processo rigoroso de revisão e comentários com os clientes para atender às necessidades práticas de produção.</span><span class="sxs-lookup"><span data-stu-id="28d44-105">API sets on the v1.0 endpoint (`https://graph.microsoft.com/v1.0`) are in general availability (GA) status, and have gone through a rigorous review-and-feedback process with customers to meet practical, production needs.</span></span> <span data-ttu-id="28d44-106">Atualizações para APIs neste ponto de extremidade são de natureza aditiva e não quebram os cenários de aplicativos existentes.</span><span class="sxs-lookup"><span data-stu-id="28d44-106">Updates to APIs on this endpoint are additive in nature and do not break existing app scenarios.</span></span>

## <a name="common-use-cases"></a><span data-ttu-id="28d44-107">Casos comuns de uso</span><span class="sxs-lookup"><span data-stu-id="28d44-107">Common use cases</span></span>

<span data-ttu-id="28d44-108">O poder do Microsoft Graph reside na fácil navegação de entidades e relacionamentos entre diferentes serviços expostos em um único ponto de extremidade REST do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="28d44-108">The power of Microsoft Graph lies in easy navigation of entities and relationships across different services exposed on a single Microsoft Graph REST endpoint.</span></span>

<span data-ttu-id="28d44-109">Vários desses serviços são projetados para permitir cenários ricos em torno de um [usuário](./resources/user.md) e em torno de um [grupo](./resources/group.md).</span><span class="sxs-lookup"><span data-stu-id="28d44-109">A number of these services are designed to enable rich scenarios around a [user](./resources/user.md) and around a [group](./resources/group.md).</span></span>

### <a name="user-centric-use-cases-in-v10"></a><span data-ttu-id="28d44-110">Casos de uso centrado no usuário na v1.0</span><span class="sxs-lookup"><span data-stu-id="28d44-110">User-centric use cases in v1.0</span></span>

1. <span data-ttu-id="28d44-111">[Obter o perfil](./api/user-get.md) e a [foto](./resources/profilephoto.md) de um usuário, Lisa.</span><span class="sxs-lookup"><span data-stu-id="28d44-111">[Get the profile](./api/user-get.md) and [photo](./resources/profilephoto.md) of a user, Lisa.</span></span>
2. <span data-ttu-id="28d44-112">[Obter as informações de perfil sobre o gerente de Lisa](./api/user-list-manager.md) e as [IDs de seus subordinados diretos](./api/user-list-directreports.md), todos armazenados no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="28d44-112">[Get the profile information about Lisa's manager](./api/user-list-manager.md) and [IDs of her direct reports](./api/user-list-directreports.md), all stored in Azure Active Directory.</span></span>
3. <span data-ttu-id="28d44-113">[Acessar os arquivos de Lisa no OneDrive for Business](./api/driveitem-list-children.md), localizar a [identidade](./resources/identityset.md) da última pessoa que modificou um [arquivo](./resources/driveitem.md) e navegar até o perfil dessa pessoa.</span><span class="sxs-lookup"><span data-stu-id="28d44-113">[Access Lisa's files on OneDrive for Business](./api/driveitem-list-children.md), find the [identity](./resources/identityset.md) of the last person who modified a [file](./resources/driveitem.md) there, and navigate to that person's profile.</span></span>
4. <span data-ttu-id="28d44-114">[Acessar o calendário de Lisa](./api/calendar-get.md) no Exchange Online e [determinar o melhor horário para Lisa se reunir com sua equipe](./api/user-findmeetingtimes.md) nas próximas duas semanas.</span><span class="sxs-lookup"><span data-stu-id="28d44-114">[Access Lisa's calendar](./api/calendar-get.md) on Exchange Online and [determine the best time for Lisa to meet with her team](./api/user-findmeetingtimes.md) in the next two weeks.</span></span>
5. <span data-ttu-id="28d44-115">[Inscrever-se](./api/subscription-post-subscriptions.md) e [acompanhar as mudanças](./api/event-delta.md) no calendário de Lisa, dizer a Lisa quando ela estiver gastando mais de 80% de seu tempo em reuniões.</span><span class="sxs-lookup"><span data-stu-id="28d44-115">[Subscribe to](./api/subscription-post-subscriptions.md) and [track changes](./api/event-delta.md) in Lisa's calendar, tell Lisa when she is spending more than 80% of her time in meetings.</span></span>
6. <span data-ttu-id="28d44-116">[Definir respostas automáticas](./api/user-update-mailboxsettings.md#example-1) quando Lisa estiver fora do escritório.</span><span class="sxs-lookup"><span data-stu-id="28d44-116">[Set automatic replies](./api/user-update-mailboxsettings.md#example-1) when Lisa is away from the office.</span></span>
7. <span data-ttu-id="28d44-117">[Receber as pessoas mais relevantes para a Lisa](./api/user-list-people.md), com base nas relações de comunicação, colaboração e negócios.</span><span class="sxs-lookup"><span data-stu-id="28d44-117">[Get the people who are most relevant to Lisa](./api/user-list-people.md), based on communication, collaboration, and business relationships.</span></span>
8. <span data-ttu-id="28d44-118">Obter a última projeção de vendas de um [gráfico](./resources/chart.md) em um arquivo do Excel no OneDrive for Business de Lisa.</span><span class="sxs-lookup"><span data-stu-id="28d44-118">Get the latest sales projection from a [chart](./resources/chart.md) in an Excel file in Lisa's OneDrive for Business.</span></span>
9. <span data-ttu-id="28d44-119">[Encontrar as tarefas atribuídas a Lisa no Planner](./api/planneruser-list-tasks.md).</span><span class="sxs-lookup"><span data-stu-id="28d44-119">[Find the tasks assigned to Lisa in Planner](./api/planneruser-list-tasks.md).</span></span>

### <a name="office-365-group-use-cases-in-v10"></a><span data-ttu-id="28d44-120">Casos de uso de grupo do Office 365 na v1.0</span><span class="sxs-lookup"><span data-stu-id="28d44-120">Office 365 group use cases in v1.0</span></span>

1. <span data-ttu-id="28d44-121">Executar um relatório sobre grupos do Office 365 em uma organização e identificar o grupo com mais [comunicação entre os membros do grupo](./api/reportroot-getoffice365groupsactivitycounts.md).</span><span class="sxs-lookup"><span data-stu-id="28d44-121">Run a report on Office 365 groups in an organization and identify the group with the most [communication among group members](./api/reportroot-getoffice365groupsactivitycounts.md).</span></span>
2. <span data-ttu-id="28d44-122">[Encontrar os planos desse grupo do Office 365](./api/plannergroup-list-plans.md) e a [atribuição de tarefas](./resources/plannerassignments.md) nesse plano.</span><span class="sxs-lookup"><span data-stu-id="28d44-122">[Find the plans of this Office 365 group](./api/plannergroup-list-plans.md), and the [assignment of tasks](./resources/plannerassignments.md) in that plan.</span></span>
3. <span data-ttu-id="28d44-123">[Iniciar uma nova conversa](./api/group-post-conversations.md) no grupo do Office 365 para determinar se os membros desejam [criar](./api/group-post-groups.md) outro grupo para compartilhar a carga de trabalho.</span><span class="sxs-lookup"><span data-stu-id="28d44-123">[Start a new conversation](./api/group-post-conversations.md) in the Office 365 group to determine if members want to [create another group](./api/group-post-groups.md) to share the workload.</span></span>
4. <span data-ttu-id="28d44-124">[Obter o bloco de anotações padrão](./api/notebook-get.md) para o grupo e [criar uma página](./api/section-post-pages.md) para anotar o resultado da investigação.</span><span class="sxs-lookup"><span data-stu-id="28d44-124">[Get the default notebook](./api/notebook-get.md) for the group and [create a page](./api/section-post-pages.md) to note the outcome of the investigation.</span></span>

## <a name="other-api-versions"></a><span data-ttu-id="28d44-125">Outras versões da API</span><span class="sxs-lookup"><span data-stu-id="28d44-125">Other API versions</span></span>

<span data-ttu-id="28d44-126">Existem atualmente 2 versões de APIs REST do Microsoft Graph - v1.0 e beta.</span><span class="sxs-lookup"><span data-stu-id="28d44-126">There are currently 2 versions of Microsoft Graph REST APIs - v1.0 and beta.</span></span>
<span data-ttu-id="28d44-127">Se você estiver interessado em APIs novas ou aprimoradas que ainda estejam no status de visualização, consulte [referência de ponto de extremidade beta do Microsoft Graph](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta).</span><span class="sxs-lookup"><span data-stu-id="28d44-127">If you're interested in new or enhanced APIs that are still in preview status, see [Microsoft Graph beta endpoint reference](/graph/api/overview?toc=./ref/toc.json&view=graph-rest-beta).</span></span> <span data-ttu-id="28d44-128">Esteja ciente de que as APIs no status de visualização estão sujeitas a alterações e podem interromper os cenários existentes sem aviso prévio.</span><span class="sxs-lookup"><span data-stu-id="28d44-128">Be aware that APIs in preview status are subject to change, and may break existing scenarios without notice.</span></span> <span data-ttu-id="28d44-129">Não obtenha uma dependência de produção de APIs no ponto de extremidade beta.</span><span class="sxs-lookup"><span data-stu-id="28d44-129">Don't take a production dependency on APIs in the beta endpoint.</span></span>

<span data-ttu-id="28d44-130">Encontre mais informações em [Suporte e controle de versão](/graph/versioning-and-support).</span><span class="sxs-lookup"><span data-stu-id="28d44-130">Find more information about [versioning and support](/graph/versioning-and-support).</span></span>

## <a name="call-the-v10-endpoint"></a><span data-ttu-id="28d44-131">Chame o ponto de extremidade do v 1.0</span><span class="sxs-lookup"><span data-stu-id="28d44-131">Call the v1.0 endpoint</span></span>

<span data-ttu-id="28d44-132">As solicitações da API do Microsoft Graph para o ponto de extremidade v1.0 usam o seguinte padrão:</span><span class="sxs-lookup"><span data-stu-id="28d44-132">Microsoft Graph API requests to the v1.0 endpoint use the following pattern:</span></span>

```
https://graph.microsoft.com/v1.0/{resource}?[query_parameters]
```

<span data-ttu-id="28d44-133">Para detalhes, consulte [Usando a API do Microsoft Graph](/graph/use-the-api).</span><span class="sxs-lookup"><span data-stu-id="28d44-133">For details, see [Use the Microsoft Graph API](/graph/use-the-api).</span></span>

## <a name="whats-new"></a><span data-ttu-id="28d44-134">Novidades</span><span class="sxs-lookup"><span data-stu-id="28d44-134">What's new</span></span>
<span data-ttu-id="28d44-135">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) no ponto de extremidade v 1.0.</span><span class="sxs-lookup"><span data-stu-id="28d44-135">Find out about the [latest new features and updates](/graph/whats-new-overview) in the v1.0 endpoint.</span></span>

## <a name="connect-with-us"></a><span data-ttu-id="28d44-136">Fale conosco</span><span class="sxs-lookup"><span data-stu-id="28d44-136">Connect with us</span></span>

<span data-ttu-id="28d44-137">Existem APIs adicionais ou recursos que você gostaria de ver no Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="28d44-137">Are there additional APIs or features you'd like to see in Microsoft Graph?</span></span> <span data-ttu-id="28d44-138">Poste novas solicitações de recursos no [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).</span><span class="sxs-lookup"><span data-stu-id="28d44-138">Post new feature requests on [UserVoice](https://officespdev.uservoice.com/forums/224641-general/filters/new?category_id=101632).</span></span>

<span data-ttu-id="28d44-139">Possui comentários para APIs existentes do Microsoft Graph?</span><span class="sxs-lookup"><span data-stu-id="28d44-139">Have feedback for existing Microsoft Graph APIs?</span></span> <span data-ttu-id="28d44-140">Conecte-se conosco em [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).</span><span class="sxs-lookup"><span data-stu-id="28d44-140">Connect with us on [Github](https://github.com/microsoftgraph/microsoft-graph-docs/issues).</span></span>
