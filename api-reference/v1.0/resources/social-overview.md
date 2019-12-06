---
title: Usar a API do Microsoft Graph para integrar a pesquisa de dados relevantes sobre pessoas em um aplicativo
description: O Microsoft Graph permite o acesso a dados úteis sobre pessoas e documentos com os quais eles interagem.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 43d2c00e9651c6bbf73e82102a36eb25efd94215
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39845032"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-intelligence-in-an-app"></a><span data-ttu-id="26b9c-103">Usar a API do Microsoft Graph para integrar a pesquisa de dados relevantes sobre pessoas em um aplicativo</span><span class="sxs-lookup"><span data-stu-id="26b9c-103">Use the Microsoft Graph API to integrate people and workplace intelligence in an app</span></span>

<span data-ttu-id="26b9c-104">O Microsoft Graph permite o acesso a dados úteis sobre pessoas e documentos com os quais eles interagem.</span><span class="sxs-lookup"><span data-stu-id="26b9c-104">Microsoft Graph enables access to useful data about people and documents they interact with.</span></span>

## <a name="aggregate-and-extract-specific-information-about-people"></a><span data-ttu-id="26b9c-105">Agregar e extraia informações específicas sobre pessoas</span><span class="sxs-lookup"><span data-stu-id="26b9c-105">Aggregate and extract specific information about people</span></span>

<span data-ttu-id="26b9c-106">Recurso: Pessoas</span><span class="sxs-lookup"><span data-stu-id="26b9c-106">Feature: People</span></span>

<span data-ttu-id="26b9c-107">Você pode usar o recurso [pessoa](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais.</span><span class="sxs-lookup"><span data-stu-id="26b9c-107">You can use the [person](../resources/person.md) resource and the People API to aggregate information about a person from across mail, contacts, and social networks.</span></span> <span data-ttu-id="26b9c-108">Os resultados são ordenados por relevância com base em vários padrões de comunicação e colaboração e em relações comerciais.</span><span class="sxs-lookup"><span data-stu-id="26b9c-108">The results are ordered by their relevance based on multiple communication and collaboration patterns and business relationships.</span></span> <span data-ttu-id="26b9c-109">A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.</span><span class="sxs-lookup"><span data-stu-id="26b9c-109">The API lets you browse, sort, select, filter, or search for persons based on your criteria.</span></span>

<span data-ttu-id="26b9c-110">Para ver cenários e exemplos, confira [Obter informações sobre pessoas relevantes](/graph/people-example).</span><span class="sxs-lookup"><span data-stu-id="26b9c-110">For scenarios and examples, see [Get information about relevant people](/graph/people-example).</span></span>

<span data-ttu-id="26b9c-111">Para usar a API, confira o seguinte:</span><span class="sxs-lookup"><span data-stu-id="26b9c-111">To use the API, see the following:</span></span>

- [<span data-ttu-id="26b9c-112">Listar pessoas</span><span class="sxs-lookup"><span data-stu-id="26b9c-112">List people</span></span>](../api/user-list-people.md)


## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a><span data-ttu-id="26b9c-113">Ajudar os usuários a obter os documentos mais relevantes para seu trabalho</span><span class="sxs-lookup"><span data-stu-id="26b9c-113">Help users get the most relevant documents for their work</span></span>

<span data-ttu-id="26b9c-114">Recurso: Ideias do documento</span><span class="sxs-lookup"><span data-stu-id="26b9c-114">Feature: Document insights</span></span>

<span data-ttu-id="26b9c-115">Usar a API insights para identificar os documentos mais relevantes para o usuário:</span><span class="sxs-lookup"><span data-stu-id="26b9c-115">Use the insights API to identify the most relevant documents for a user:</span></span>

- <span data-ttu-id="26b9c-116">Listar documentos [mais populares](../api/insights-list-trending.md) de um usuário</span><span class="sxs-lookup"><span data-stu-id="26b9c-116">List documents [trending around](../api/insights-list-trending.md) a user</span></span>
- <span data-ttu-id="26b9c-117">Listar documentos [usados por](../api/insights-list-used.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="26b9c-117">List documents [used by](../api/insights-list-used.md) a user</span></span>
- <span data-ttu-id="26b9c-118">Listar documentos [compartilhados com ou por](../api/insights-list-shared.md) um usuário</span><span class="sxs-lookup"><span data-stu-id="26b9c-118">List documents [shared with or shared by](../api/insights-list-shared.md) a user</span></span>
