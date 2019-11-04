---
title: Usar a API do Microsoft Graph para integrar a inteligência de pessoas e de local de trabalho em um aplicativo
description: O Microsoft Graph permite o acesso a dados pessoais e do local de trabalho úteis e dá suporte a gestos sociais no contexto social de um usuário.
localization_priority: Priority
author: simonhult
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: f87f3032f58475eed95507b4e436735e5c484fc4
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939359"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-and-workplace-intelligence-in-an-app"></a><span data-ttu-id="35d0b-103">Usar a API do Microsoft Graph para integrar a inteligência de pessoas e de local de trabalho em um aplicativo</span><span class="sxs-lookup"><span data-stu-id="35d0b-103">Use the Microsoft Graph API to integrate social and workplace intelligence in an app</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35d0b-104">O Microsoft Graph permite o acesso a dados pessoais e do local de trabalho para pessoas e dá suporte a gestos sociais no contexto social de um usuário.</span><span class="sxs-lookup"><span data-stu-id="35d0b-104">Microsoft Graph enables access to people and workplace data for people, and supports gestures in a user's social context.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="35d0b-105">Agregar e extraia informações específicas sobre pessoas</span><span class="sxs-lookup"><span data-stu-id="35d0b-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="35d0b-106">Use o recurso [person](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="35d0b-106">Use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="35d0b-107">Os resultados são ordenados por sua relevância com base em várias relações de comunicação, colaboração e comerciais.</span><span class="sxs-lookup"><span data-stu-id="35d0b-107">The results are ordered by their relevance based on multiple communication, collaboration, and business relationships.</span></span> <span data-ttu-id="35d0b-108">A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.</span><span class="sxs-lookup"><span data-stu-id="35d0b-108">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

- [<span data-ttu-id="35d0b-109">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="35d0b-109">List people</span></span>](../api/user-list-people.md)

## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="35d0b-110">Ajudar os usuários a obter os documentos mais relevantes para seu trabalho</span><span class="sxs-lookup"><span data-stu-id="35d0b-110">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="35d0b-111">Usar a API insights para identificar os documentos mais relevantes para o usuário:</span><span class="sxs-lookup"><span data-stu-id="35d0b-111">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="35d0b-112">Listar documentos [mais populares](../api/insights-list-trending.md) de um usuário</span><span class="sxs-lookup"><span data-stu-id="35d0b-112">List the items [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="35d0b-113">Listar documentos [usados por](../api/insights-list-used.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="35d0b-113">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="35d0b-114">Listar documentos [compartilhados com ou por](../api/insights-list-shared.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="35d0b-114">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>

## <a name="help-users-gain-insights-into-their-work-patterns"></a><span data-ttu-id="35d0b-115">Ajudar os usuários a obter informações sobre seus padrões de trabalho</span><span class="sxs-lookup"><span data-stu-id="35d0b-115">Help users gain insights into their work patterns</span></span>

<span data-ttu-id="35d0b-116">Usar a API de análise para obter estatísticas de atividade e configurações relacionadas para um usuários:</span><span class="sxs-lookup"><span data-stu-id="35d0b-116">Use the analytics API to get activity statistics and related settings for a user:</span></span>

- <span data-ttu-id="35d0b-117">[configurações](../resources/settings.md): Para a API de análise retornar os resultados para um usuários, as configurações de análise de usuário atuais devem mostrar uma licença válida do MyAnalytics, ser aceitas no uso do MyAnalytics e ter uma caixa de correio hospedada na nuvem habilitada para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="35d0b-117">[settings](../resources/settings.md): For the analytics API to return results for a user, the current user analytics settings must show a valid MyAnalytics license, be opted in to using MyAnalytics, and have a cloud-hosted mailbox that’s graph-enabled.</span></span>
- <span data-ttu-id="35d0b-118">[activityStatistics](../resources/activitystatistics.md): Obtém dados para a última semana concluída (ou o intervalo de tempo especificado) das atividades do Office 365 em que um usuário gastou tempo, incluindo o número de horas gastas em [chamadas](callactivitystatistics.md), [conversas (mensagens instantâneas)](chatactivitystatistics.md), [email](emailactivitystatistics.md) e [reuniões](meetingactivitystatistics.md) durante e fora das horas de trabalho e o número de horas disponíveis para o [trabalho prioritário](focusactivitystatistics.md).</span><span class="sxs-lookup"><span data-stu-id="35d0b-118">[activityStatistics](../resources/activitystatistics.md): Gets data for the last complete week (or the specified time range) for the Office 365 activities that a user spent time on, including the number of hours spent on [calls](callactivitystatistics.md), [chats (instant messages)](chatactivitystatistics.md), [email](emailactivitystatistics.md), and [meetings](meetingactivitystatistics.md) during and outside of working hours and the number of hours available for [focused work](focusactivitystatistics.md).</span></span>

## <a name="manage--mentions"></a><span data-ttu-id="35d0b-119">Gerenciar as @menções</span><span class="sxs-lookup"><span data-stu-id="35d0b-119">Manage @-Mentions</span></span>

<span data-ttu-id="35d0b-120">Chamar um destinatário para notificar e atrair a atenção do destinatário em uma mensagem é um gesto social comum.</span><span class="sxs-lookup"><span data-stu-id="35d0b-120">Calling out a recipient to notify and get the recipient's attention in a message is a common social gesture.</span></span>
<span data-ttu-id="35d0b-121">O recurso [menção](../resources/mention.md) e a API de Menções fornecem um mecanismo simplificado para marcar um destinatário em uma [mensagem](../resources/message.md), receber todas as mensagens nas quais um usuário é notificado usando uma @menção ou receber cada menção em uma mensagem.</span><span class="sxs-lookup"><span data-stu-id="35d0b-121">The [mention](../resources/mention.md) resource and the Mentions API provide a light-weight mechanism to call out a recipient in a [message](../resources/message.md), get all the messages in which a user is notified using an @-mention, or get each mention in a message.</span></span>

<!--
Include the next sentence when supporting events.

**Mention** is also supported by [Event](../resources/event.md).

-->

- <span data-ttu-id="35d0b-122">Criar menções em uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="35d0b-122">Create mentions in a new message</span></span>

  - [<span data-ttu-id="35d0b-123">Criar e enviar menções como parte de uma nova mensagem</span><span class="sxs-lookup"><span data-stu-id="35d0b-123">Create and send mentions as part of a new message</span></span>](../api/user-sendmail.md#request-2)
  - [<span data-ttu-id="35d0b-124">Criar menções como parte de um rascunho da mensagem</span><span class="sxs-lookup"><span data-stu-id="35d0b-124">Create mentions as part of a message draft</span></span>](../api/user-post-messages.md#request-2)

- <span data-ttu-id="35d0b-125">Obter informações sobre menções em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="35d0b-125">Get information about mentions in a message</span></span>

  - [<span data-ttu-id="35d0b-126">Obter todas as mensagens na caixa de correio do usuário conectado que mencionou o usuário</span><span class="sxs-lookup"><span data-stu-id="35d0b-126">Get all the messages in the signed-in user's mailbox that mention the user</span></span>](../api/user-list-messages.md#request-2)
  - [<span data-ttu-id="35d0b-127">Obter os detalhes de cada menção em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="35d0b-127">Get details of each mention in a message</span></span>](../api/message-get.md#request-2)

- <span data-ttu-id="35d0b-128">[Excluir uma menção](../api/message-delete.md#request-2) em uma mensagem</span><span class="sxs-lookup"><span data-stu-id="35d0b-128">[Delete a mention](../api/message-delete.md#request-2) in a message</span></span>

## <a name="help-users-contextualize-others-in-their-organization"></a><span data-ttu-id="35d0b-129">Ajudar os usuários a contextualizarem outras pessoas em sua organização</span><span class="sxs-lookup"><span data-stu-id="35d0b-129">Help users contextualize others in their organization</span></span>

<span data-ttu-id="35d0b-130">As pessoas que procuram contextualizar outras na organização geralmente exibem o perfil ou o cartão de perfil de uma pessoa.</span><span class="sxs-lookup"><span data-stu-id="35d0b-130">People who seek to contextualize others within their organization commonly view a person's profile or profile card.</span></span> 

<span data-ttu-id="35d0b-131">O recurso [perfil](../resources/profile.md) é uma avançada fonte de informações sobre as pessoas dentro de um locatário e proporciona um mecanismo leve para armazenar e recuperar informações sobre alguém.</span><span class="sxs-lookup"><span data-stu-id="35d0b-131">The [profile](../resources/profile.md) resource is a rich source of information about people within a tenant and provides a lightweight mechanism for storing and retrieving information about a person.</span></span> 
