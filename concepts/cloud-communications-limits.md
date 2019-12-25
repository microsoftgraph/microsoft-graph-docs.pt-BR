---
title: Limites de API de comunicação em nuvem no Microsoft Graph
description: Contém informações sobre os limites das APIs de comunicação em nuvem
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 0338c7b37a58da66aac75430234a4b1df56b07b1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871552"
---
# <a name="cloud-communication-api-limits-in-microsoft-graph"></a><span data-ttu-id="8a22c-103">Limites de API de comunicação em nuvem no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a22c-103">Cloud communication API limits in Microsoft Graph</span></span>

<span data-ttu-id="8a22c-104">Este artigo descreve as limitações das APIs de comunicação em nuvem.</span><span class="sxs-lookup"><span data-stu-id="8a22c-104">This article describes limitations to the cloud communications APIs.</span></span> <span data-ttu-id="8a22c-105">Esses limites ajudam a garantir que a plataforma seja estável, confiável e segura.</span><span class="sxs-lookup"><span data-stu-id="8a22c-105">These limits help to ensure that the platform is stable, reliable, and secure.</span></span> <span data-ttu-id="8a22c-106">Observe que essas limitações estão sujeitas a alterações no futuro.</span><span class="sxs-lookup"><span data-stu-id="8a22c-106">Note that these limitations are subject to change in the future.</span></span> 

><span data-ttu-id="8a22c-107">**Observação:** Quando o limite é atingido, tentar fazer mais solicitações de API resultará em um HTTP `429 Error`.</span><span class="sxs-lookup"><span data-stu-id="8a22c-107">**Note:** When the limit is reached, attempting to make more API requests will result in an HTTP `429 Error`.</span></span>

| <span data-ttu-id="8a22c-108">API</span><span class="sxs-lookup"><span data-stu-id="8a22c-108">API</span></span>      | <span data-ttu-id="8a22c-109">Limitações</span><span class="sxs-lookup"><span data-stu-id="8a22c-109">Limitations</span></span>    |
| :------------- | :----------: |
|  <span data-ttu-id="8a22c-110">Chamadas</span><span class="sxs-lookup"><span data-stu-id="8a22c-110">Calls</span></span> | <span data-ttu-id="8a22c-111">10.000 chamadas/mês e 100 chamadas simultâneas</span><span class="sxs-lookup"><span data-stu-id="8a22c-111">10,000 calls/month and 100 concurrent calls</span></span>   |
| <span data-ttu-id="8a22c-112">Reuniões</span><span class="sxs-lookup"><span data-stu-id="8a22c-112">Meetings</span></span>   | <span data-ttu-id="8a22c-113">2000 reuniões/usuários por mês</span><span class="sxs-lookup"><span data-stu-id="8a22c-113">2000 meetings/user each month</span></span> |
| <span data-ttu-id="8a22c-114">Presença (visualização)</span><span class="sxs-lookup"><span data-stu-id="8a22c-114">Presence (preview)</span></span>   | <span data-ttu-id="8a22c-115">2 solicitações/segundo</span><span class="sxs-lookup"><span data-stu-id="8a22c-115">2 requests/second</span></span> |

## <a name="see-also"></a><span data-ttu-id="8a22c-116">Confira também</span><span class="sxs-lookup"><span data-stu-id="8a22c-116">See also</span></span>

- [<span data-ttu-id="8a22c-117">Trabalhar com a API de comunicação</span><span class="sxs-lookup"><span data-stu-id="8a22c-117">Working with the communications API</span></span>](/graph/api/resources/communications-api-overview?view=graph-rest-beta)
