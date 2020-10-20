---
title: Trabalhar com a API de registros de chamadas no Microsoft Graph
description: A API de registros de chamadas do Microsoft Graph permite recuperar dados de uso e de diagnóstico das chamadas e reuniões on-line dentro da organização.
author: williamlooney
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 56b81ceb902701c0125cee6e1b0f20087bbeac50
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48601577"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a><span data-ttu-id="355ce-103">Trabalhar com a API de registros de chamadas no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="355ce-103">Working with the call records API in Microsoft Graph</span></span>

<span data-ttu-id="355ce-104">Os registros das chamadas fornecem informações de uso e diagnóstico das chamadas e reuniões on-line que ocorrem na sua organização ao usar o Microsoft Teams ou o Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="355ce-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="355ce-105">Você pode usar as APIs de registros de chamadas para se inscrever nos registros de chamadas e procurar registros de chamadas por IDs.</span><span class="sxs-lookup"><span data-stu-id="355ce-105">You can use the call records APIs to subscribe to call records and look up call records by IDs.</span></span>

<span data-ttu-id="355ce-106">A API de registros de chamadas é definida no subnamespace OData, `microsoft.graph.callRecords`.</span><span class="sxs-lookup"><span data-stu-id="355ce-106">The call records API is defined in the OData sub-namespace, `microsoft.graph.callRecords`.</span></span>

## <a name="key-resource-types"></a><span data-ttu-id="355ce-107">Principais tipos de recursos</span><span class="sxs-lookup"><span data-stu-id="355ce-107">Key resource types</span></span>

| <span data-ttu-id="355ce-108">Resource</span><span class="sxs-lookup"><span data-stu-id="355ce-108">Resource</span></span> | <span data-ttu-id="355ce-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="355ce-109">Methods</span></span> |
| :-- | :-- |
| [<span data-ttu-id="355ce-110">callRecord</span><span class="sxs-lookup"><span data-stu-id="355ce-110">callRecord</span></span>](callrecords-callrecord.md) | [<span data-ttu-id="355ce-111">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="355ce-111">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |
| [<span data-ttu-id="355ce-112">sessão</span><span class="sxs-lookup"><span data-stu-id="355ce-112">session</span></span>](callrecords-session.md) | [<span data-ttu-id="355ce-113">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="355ce-113">Get callRecord</span></span>](../api/callrecords-callrecord-get.md)<br />[<span data-ttu-id="355ce-114">Listar sessões</span><span class="sxs-lookup"><span data-stu-id="355ce-114">List sessions</span></span>](../api/callrecords-session-list.md) |
| [<span data-ttu-id="355ce-115">segmento</span><span class="sxs-lookup"><span data-stu-id="355ce-115">segment</span></span>](callrecords-segment.md) | [<span data-ttu-id="355ce-116">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="355ce-116">Get callRecord</span></span>](../api/callrecords-callrecord-get.md)<br />[<span data-ttu-id="355ce-117">Listar sessões</span><span class="sxs-lookup"><span data-stu-id="355ce-117">List sessions</span></span>](../api/callrecords-session-list.md) |

## <a name="call-record-structure"></a><span data-ttu-id="355ce-118">Estrutura do registro de chamadas</span><span class="sxs-lookup"><span data-stu-id="355ce-118">Call record structure</span></span>

<span data-ttu-id="355ce-119">A entidade [callRecord](callrecords-callrecord.md) representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião on-line.</span><span class="sxs-lookup"><span data-stu-id="355ce-119">The [callRecord](callrecords-callrecord.md) entity represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

<span data-ttu-id="355ce-120">Uma chamada ponto a ponto contém uma única [sessão](callrecords-session.md) entre os dois participantes da chamada.</span><span class="sxs-lookup"><span data-stu-id="355ce-120">A peer-to-peer call contains a single [session](callrecords-session.md) between the two participants in the call.</span></span> <span data-ttu-id="355ce-121">As chamadas de grupo contêm uma ou mais entidades de **sessão**.</span><span class="sxs-lookup"><span data-stu-id="355ce-121">Group calls contain one or more **session** entities.</span></span> <span data-ttu-id="355ce-122">Em uma chamada de grupo, cada **sessão** fica entre o participante e um ponto de extremidade do serviço.</span><span class="sxs-lookup"><span data-stu-id="355ce-122">In a group call, each **session** is between the participant and a service endpoint.</span></span>

<span data-ttu-id="355ce-123">Cada **sessão** contém uma ou mais entidades do [segmento](callrecords-segment.md).</span><span class="sxs-lookup"><span data-stu-id="355ce-123">Each **session** contains one or more [segment](callrecords-segment.md) entities.</span></span> <span data-ttu-id="355ce-124">Um **segmento** representa um link de mídia entre dois [pontos de extremidade](callrecords-endpoint.md).</span><span class="sxs-lookup"><span data-stu-id="355ce-124">A **segment** represents a media link between two [endpoints](callrecords-endpoint.md).</span></span> <span data-ttu-id="355ce-125">Para a maioria das chamadas, apenas um **segmento** estará presente em cada **sessão**. Entretanto, às vezes, poderá haver um ou mais **pontos de extremidade** intermediários.</span><span class="sxs-lookup"><span data-stu-id="355ce-125">For most calls, only one **segment** will be present for each **session**, however sometimes there may be one or more intermediate **endpoints**.</span></span>

![Imagem de uma estrutura de dados que representa um registro de chamada concluída](/graph/images/callrecords-structure.png)

<span data-ttu-id="355ce-127">No diagrama acima, o número denota quantas crianças de cada tipo podem estar presentes.</span><span class="sxs-lookup"><span data-stu-id="355ce-127">In the diagram above, the numbers denote how many children of each type can be present.</span></span> <span data-ttu-id="355ce-128">Por exemplo: uma relação 1..N entre um **callRecord** e uma **sessão** significa que uma instância **callRecord** pode conter uma ou mais instâncias da **sessão**.</span><span class="sxs-lookup"><span data-stu-id="355ce-128">For example, a 1..N relationship between a **callRecord** and a **session** means one **callRecord** instance can contain one or more **session** instances.</span></span> <span data-ttu-id="355ce-129">Da mesma forma, uma relação 1..N entre um **segmento** e uma **mídia** significa que uma instância do **segmento** pode conter um ou mais fluxos de [mídia](callrecords-media.md).</span><span class="sxs-lookup"><span data-stu-id="355ce-129">Similarly, a 1..N relationship between a **segment** and a **media** means one **segment** instance can contain one or more [media](callrecords-media.md) streams.</span></span>

## <a name="see-also"></a><span data-ttu-id="355ce-130">Também consulte</span><span class="sxs-lookup"><span data-stu-id="355ce-130">See also</span></span>

- [<span data-ttu-id="355ce-131">Assinaturas do Webhook</span><span class="sxs-lookup"><span data-stu-id="355ce-131">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-1.0)

