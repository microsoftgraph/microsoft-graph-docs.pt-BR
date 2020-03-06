---
title: Trabalhar com a API de registros de chamadas no Microsoft Graph
description: A API de registros de chamadas do Microsoft Graph permite recuperar dados de uso e de diagnóstico das chamadas e reuniões on-line dentro da organização.
author: stephenjust
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 9b48b3d7f0265c44bc62c3ee2182353343692a10
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507800"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a><span data-ttu-id="0b041-103">Trabalhar com a API de registros de chamadas no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="0b041-103">Working with the call records API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b041-104">Os registros das chamadas fornecem informações de uso e diagnóstico das chamadas e reuniões on-line que ocorrem na sua organização ao usar o Microsoft Teams ou o Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="0b041-104">Call records provide usage and diagnostic information about the calls and online meetings that occur within your organization when using Microsoft Teams or Skype for Business.</span></span> <span data-ttu-id="0b041-105">Você pode usar as APIs de registros de chamadas para se inscrever nos registros de chamadas e procurar registros de chamadas por IDs.</span><span class="sxs-lookup"><span data-stu-id="0b041-105">You can use the call records APIs to subscribe to call records and look up call records by IDs.</span></span>

<span data-ttu-id="0b041-106">A API de registros de chamadas é definida no subnamespace OData, `microsoft.graph.callRecords`.</span><span class="sxs-lookup"><span data-stu-id="0b041-106">The call records API is defined in the OData sub-namespace, `microsoft.graph.callRecords`.</span></span>

## <a name="key-resource-types"></a><span data-ttu-id="0b041-107">Principais tipos de recursos</span><span class="sxs-lookup"><span data-stu-id="0b041-107">Key resource types</span></span>

| <span data-ttu-id="0b041-108">Resource</span><span class="sxs-lookup"><span data-stu-id="0b041-108">Resource</span></span> | <span data-ttu-id="0b041-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="0b041-109">Methods</span></span> |
| :-- | :-- |
| [<span data-ttu-id="0b041-110">callRecord</span><span class="sxs-lookup"><span data-stu-id="0b041-110">callRecord</span></span>](callrecords-callrecord.md) | [<span data-ttu-id="0b041-111">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="0b041-111">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |
| [<span data-ttu-id="0b041-112">sessão</span><span class="sxs-lookup"><span data-stu-id="0b041-112">session</span></span>](callrecords-session.md) | [<span data-ttu-id="0b041-113">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="0b041-113">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |
| [<span data-ttu-id="0b041-114">segmento</span><span class="sxs-lookup"><span data-stu-id="0b041-114">segment</span></span>](callrecords-segment.md) | [<span data-ttu-id="0b041-115">Obter callRecord</span><span class="sxs-lookup"><span data-stu-id="0b041-115">Get callRecord</span></span>](../api/callrecords-callrecord-get.md) |

## <a name="call-record-structure"></a><span data-ttu-id="0b041-116">Estrutura do registro de chamadas</span><span class="sxs-lookup"><span data-stu-id="0b041-116">Call record structure</span></span>

<span data-ttu-id="0b041-117">A entidade [callRecord](callrecords-callrecord.md) representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião on-line.</span><span class="sxs-lookup"><span data-stu-id="0b041-117">The [callRecord](callrecords-callrecord.md) entity represents a single peer-to-peer call or a group call between multiple participants, sometimes referred to as an online meeting.</span></span>

<span data-ttu-id="0b041-118">Uma chamada ponto a ponto contém uma única [sessão](callrecords-session.md) entre os dois participantes da chamada.</span><span class="sxs-lookup"><span data-stu-id="0b041-118">A peer-to-peer call contains a single [session](callrecords-session.md) between the two participants in the call.</span></span> <span data-ttu-id="0b041-119">As chamadas de grupo contêm uma ou mais entidades de **sessão**.</span><span class="sxs-lookup"><span data-stu-id="0b041-119">Group calls contain one or more **session** entities.</span></span> <span data-ttu-id="0b041-120">Em uma chamada de grupo, cada **sessão** fica entre o participante e um ponto de extremidade do serviço.</span><span class="sxs-lookup"><span data-stu-id="0b041-120">In a group call, each **session** is between the participant and a service endpoint.</span></span>

<span data-ttu-id="0b041-121">Cada **sessão** contém uma ou mais entidades do [segmento](callrecords-segment.md).</span><span class="sxs-lookup"><span data-stu-id="0b041-121">Each **session** contains one or more [segment](callrecords-segment.md) entities.</span></span> <span data-ttu-id="0b041-122">Um **segmento** representa um link de mídia entre dois [pontos de extremidade](callrecords-endpoint.md).</span><span class="sxs-lookup"><span data-stu-id="0b041-122">A **segment** represents a media link between two [endpoints](callrecords-endpoint.md).</span></span> <span data-ttu-id="0b041-123">Para a maioria das chamadas, apenas um **segmento** estará presente em cada **sessão**. Entretanto, às vezes, poderá haver um ou mais **pontos de extremidade** intermediários.</span><span class="sxs-lookup"><span data-stu-id="0b041-123">For most calls, only one **segment** will be present for each **session**, however sometimes there may be one or more intermediate **endpoints**.</span></span>

![Imagem de uma estrutura de dados que representa um registro de chamada concluída](/graph/images/callrecords-structure.png)

<span data-ttu-id="0b041-125">No diagrama acima, o número denota quantas crianças de cada tipo podem estar presentes.</span><span class="sxs-lookup"><span data-stu-id="0b041-125">In the diagram above, the numbers denote how many children of each type can be present.</span></span> <span data-ttu-id="0b041-126">Por exemplo: uma relação 1..N entre um **callRecord** e uma **sessão** significa que uma instância **callRecord** pode conter uma ou mais instâncias da **sessão**.</span><span class="sxs-lookup"><span data-stu-id="0b041-126">For example, a 1..N relationship between a **callRecord** and a **session** means one **callRecord** instance can contain one or more **session** instances.</span></span> <span data-ttu-id="0b041-127">Da mesma forma, uma relação 1..N entre um **segmento** e uma **mídia** significa que uma instância do **segmento** pode conter um ou mais fluxos de [mídia](callrecords-media.md).</span><span class="sxs-lookup"><span data-stu-id="0b041-127">Similarly, a 1..N relationship between a **segment** and a **media** means one **segment** instance can contain one or more [media](callrecords-media.md) streams.</span></span>

## <a name="see-also"></a><span data-ttu-id="0b041-128">Também consulte</span><span class="sxs-lookup"><span data-stu-id="0b041-128">See also</span></span>

- [<span data-ttu-id="0b041-129">Assinaturas do Webhook</span><span class="sxs-lookup"><span data-stu-id="0b041-129">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-beta)
