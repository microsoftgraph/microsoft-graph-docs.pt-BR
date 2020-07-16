---
title: Usar a API do Microsoft Graph para integrar a inteligência de pessoas e de local de trabalho em um aplicativo
description: O Microsoft Graph permite o acesso a dados úteis sobre pessoas, seu perfil, documentos dos quais eles interagem e padrões de trabalho e oferece suporte a gestos no contexto social de um usuário.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: d1e1f49125aa8959c1cdd6b2f47cc5c4ff81d962
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050964"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="15087-103">Usar a API do Microsoft Graph para integrar a inteligência de pessoas e de local de trabalho em um aplicativo</span><span class="sxs-lookup"><span data-stu-id="15087-103">Use the Microsoft Graph API to integrate people and workplace intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="15087-104">O Microsoft Graph permite o acesso a dados úteis sobre pessoas, seu perfil, documentos dos quais eles interagem e padrões de trabalho e oferece suporte a gestos no contexto social de um usuário.</span><span class="sxs-lookup"><span data-stu-id="15087-104">Microsoft Graph enables access to useful data about people, their profile, documents they interact with, and work patterns, and supports gestures in a user's social context.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="15087-105">Agregar e extraia informações específicas sobre pessoas</span><span class="sxs-lookup"><span data-stu-id="15087-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="15087-106">Recurso: Pessoas</span><span class="sxs-lookup"><span data-stu-id="15087-106">Feature: People</span></span>

<span data-ttu-id="15087-107">Use o recurso [person](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="15087-107">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="15087-108">Os resultados são ordenados por sua relevância com base em várias relações de comunicação, colaboração e comerciais.</span><span class="sxs-lookup"><span data-stu-id="15087-108">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="15087-109">A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.</span><span class="sxs-lookup"><span data-stu-id="15087-109">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="15087-110">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="15087-110">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-contextualize-others-in-their-organization"></a><span data-ttu-id="15087-111">Ajudar os usuários a contextualizarem outras pessoas em sua organização</span><span class="sxs-lookup"><span data-stu-id="15087-111">Help users contextualize others in their organization</span></span>

<span data-ttu-id="15087-112">Recurso: Perfil (visualização)</span><span class="sxs-lookup"><span data-stu-id="15087-112">Feature: Profile (preview)</span></span>

<span data-ttu-id="15087-113">As pessoas que procuram contextualizar outras na organização geralmente exibem o perfil ou o cartão de perfil de uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="15087-113">People who seek to contextualize others within their organization commonly view a person's profile or profile card.</span></span> 

<span data-ttu-id="15087-114">O recurso [perfil](../resources/profile.md) é uma avançada fonte de informações sobre as pessoas dentro de um locatário e proporciona um mecanismo leve para armazenar e recuperar informações sobre alguém.</span><span class="sxs-lookup"><span data-stu-id="15087-114">The [profile](../resources/profile.md) resource is a rich source of information about people within a tenant and provides a lightweight mechanism for storing and retrieving information about a person.</span></span> 

## <a name="personalize-people-experiences-within-your-organization"></a><span data-ttu-id="15087-115">Personalizar experiências de pessoas em sua organização</span><span class="sxs-lookup"><span data-stu-id="15087-115">Personalize people experiences within your organization</span></span>

<span data-ttu-id="15087-116">Recurso: personalização do cartão de perfil (versão prévia)</span><span class="sxs-lookup"><span data-stu-id="15087-116">Feature: Profile card customization (preview)</span></span>

<span data-ttu-id="15087-117">Fornece a capacidade de um administrador personalizar as informações mostradas no cartão de perfil usado no Microsoft 365 em sua organização.</span><span class="sxs-lookup"><span data-stu-id="15087-117">Provides the ability for an administrator to customize the information shown on the profile card used across Microsoft 365 within their organization.</span></span>

<span data-ttu-id="15087-118">O recurso [profileCardProperty](../resources/profileCardProperty.md) representa um atributo de um usuário no cartão de perfil do Microsoft 365 para que uma organização alcance uma experiência de pessoas compartilhada.</span><span class="sxs-lookup"><span data-stu-id="15087-118">The [profileCardProperty](../resources/profileCardProperty.md) resource represents an attribute of a user on the Microsoft 365 profile card for an organization to surface in a shared, people experience.</span></span>

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="15087-119">Ajudar os usuários a obter os documentos mais relevantes para seu trabalho</span><span class="sxs-lookup"><span data-stu-id="15087-119">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="15087-120">Recurso: Ideias do documento</span><span class="sxs-lookup"><span data-stu-id="15087-120">Feature: Document insights</span></span>

<span data-ttu-id="15087-121">Usar a API insights para identificar os documentos mais relevantes para o usuário:</span><span class="sxs-lookup"><span data-stu-id="15087-121">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="15087-122">Listar documentos [mais populares](../api/insights-list-trending.md) de um usuário</span><span class="sxs-lookup"><span data-stu-id="15087-122">List documents [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="15087-123">Listar documentos [usados por](../api/insights-list-used.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="15087-123">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="15087-124">Listar documentos [compartilhados com ou por](../api/insights-list-shared.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="15087-124">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="15087-125">Gerenciar as @menções</span><span class="sxs-lookup"><span data-stu-id="15087-125">Manage @-Mentions</span></span>

<span data-ttu-id="15087-126">Recurso: @-menções (visualização)</span><span class="sxs-lookup"><span data-stu-id="15087-126">Feature: @-mentions (preview)</span></span>

<span data-ttu-id="15087-127">Chamar um destinatário para notificar e atrair a atenção do destinatário em uma mensagem é um gesto social comum.</span><span class="sxs-lookup"><span data-stu-id="15087-127">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="15087-128">O recurso [menção](../resources/mention.md) e a API de Menções fornecem um mecanismo simplificado para marcar um destinatário em uma [mensagem](../resources/message.md), receber todas as mensagens nas quais um usuário é notificado usando uma @menção ou receber cada menção em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="15087-128">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="15087-129">Criar menções em uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="15087-129">Create mentions in a new message</span></span>

  - [<span data-ttu-id="15087-130">Criar e enviar menções como parte de uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="15087-130">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="15087-131">Criar menções como parte de um rascunho da mensagem</span><span class="sxs-lookup"><span data-stu-id="15087-131">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="15087-132">Obter informações sobre menções em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="15087-132">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="15087-133">Obter todas as mensagens na caixa de correio do usuário conectado que mencionou o usuário</span><span class="sxs-lookup"><span data-stu-id="15087-133">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="15087-134">Obter os detalhes de cada menção em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="15087-134">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="15087-135">[Excluir uma menção](../api/message-delete.md#request-2) em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="15087-135">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>


## <a name="help-users-gain-insights-into-their-work-patterns"></a><span data-ttu-id="15087-136">Ajudar os usuários a obter informações sobre seus padrões de trabalho</span><span class="sxs-lookup"><span data-stu-id="15087-136">Help users gain insights into their work patterns</span></span>

<span data-ttu-id="15087-137">Recurso: Análise (visualização)</span><span class="sxs-lookup"><span data-stu-id="15087-137">Feature: Analytics (preview)</span></span>

<span data-ttu-id="15087-138">Usar a API de análise para obter estatísticas de atividade e configurações relacionadas para um usuários:</span><span class="sxs-lookup"><span data-stu-id="15087-138">Use the analytics API to get activity statistics and related settings for a user:</span></span>

- <span data-ttu-id="15087-139">[configurações](../resources/settings.md): Para a API de análise retornar os resultados para um usuários, as configurações de análise de usuário atuais devem mostrar uma licença válida do MyAnalytics, ser aceitas no uso do MyAnalytics e ter uma caixa de correio hospedada na nuvem habilitada para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="15087-139">[settings](../resources/settings.md): For the analytics API to return results for a user, the current user analytics settings must show a valid MyAnalytics license, be opted in to using MyAnalytics, and have a cloud-hosted mailbox that’s graph-enabled.</span></span>
- <span data-ttu-id="15087-140">[activityStatistics](../resources/activitystatistics.md): Obtém os dados da última semana completa (ou do intervalo de tempo especificado) para as atividades do Microsoft 365 nas quais um usuário gastou tempo, incluindo o número de horas gastas em [chamadas](callactivitystatistics.md), [chats (mensagens instantâneas)](chatactivitystatistics.md), [email](emailactivitystatistics.md)e [reuniões](meetingactivitystatistics.md) durante e fora do horário de trabalho e o número de horas disponíveis para [trabalho focado](focusactivitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="15087-140">[activityStatistics](../resources/activitystatistics.md): Gets data for the last complete week (or the specified time range) for the Microsoft 365 activities that a user spent time on, including the number of hours spent on [calls](callactivitystatistics.md), [chats (instant messages)](chatactivitystatistics.md), [email](emailactivitystatistics.md), and [meetings](meetingactivitystatistics.md) during and outside of working hours and the number of hours available for [focused work](focusactivitystatistics.md).</span></span>

## <a name="whats-new"></a><span data-ttu-id="15087-141">Novidades</span><span class="sxs-lookup"><span data-stu-id="15087-141">What's new</span></span>
<span data-ttu-id="15087-142">Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para esses conjuntos de API.</span><span class="sxs-lookup"><span data-stu-id="15087-142">Find out about the [latest new features and updates](/graph/whats-new-overview) for these API sets.</span></span>