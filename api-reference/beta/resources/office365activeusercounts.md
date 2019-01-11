---
title: tipo de recurso de office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.openlocfilehash: 887f9b08d7f46aac023fbd0f34e6174e5f422760
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882716"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="d5ef1-103">tipo de recurso de office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="d5ef1-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d5ef1-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d5ef1-104">Properties</span></span>

| <span data-ttu-id="d5ef1-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d5ef1-105">Property</span></span>          | <span data-ttu-id="d5ef1-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d5ef1-106">Type</span></span>   | <span data-ttu-id="d5ef1-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5ef1-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d5ef1-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d5ef1-108">reportRefreshDate</span></span> | <span data-ttu-id="d5ef1-109">Data</span><span class="sxs-lookup"><span data-stu-id="d5ef1-109">Date</span></span>   | <span data-ttu-id="d5ef1-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d5ef1-111">office365</span><span class="sxs-lookup"><span data-stu-id="d5ef1-111">office365</span></span>         | <span data-ttu-id="d5ef1-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ef1-112">Int64</span></span>  | <span data-ttu-id="d5ef1-113">O número de usuários ativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-113">The number of active users in Office 365.</span></span> <span data-ttu-id="d5ef1-114">Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype For Business, Yammer e Teams da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="d5ef1-115">Você pode encontrar a definição de usuário ativo para cada produto na descrição do respectivas propriedades.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="d5ef1-116">Exchange</span><span class="sxs-lookup"><span data-stu-id="d5ef1-116">exchange</span></span>          | <span data-ttu-id="d5ef1-117">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ef1-117">Int64</span></span>  | <span data-ttu-id="d5ef1-118">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-118">The number of active users in Exchange.</span></span> <span data-ttu-id="d5ef1-119">Qualquer usuário que pode ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="d5ef1-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="d5ef1-120">oneDrive</span></span>          | <span data-ttu-id="d5ef1-121">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ef1-121">Int64</span></span>  | <span data-ttu-id="d5ef1-122">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="d5ef1-123">Qualquer usuário que são exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="d5ef1-124">sharePoint</span><span class="sxs-lookup"><span data-stu-id="d5ef1-124">sharePoint</span></span>        | <span data-ttu-id="d5ef1-125">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ef1-125">Int64</span></span>  | <span data-ttu-id="d5ef1-126">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="d5ef1-127">Qualquer usuário que exibidos ou editados arquivos, internamente de arquivos compartilhados ou sincronizados arquivos externamente ou exibidos páginas do SharePoint é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="d5ef1-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="d5ef1-128">skypeForBusiness</span></span>  | <span data-ttu-id="d5ef1-129">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ef1-129">Int64</span></span>  | <span data-ttu-id="d5ef1-130">O número de usuários ativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="d5ef1-131">Qualquer usuário que organizou participou de conferências ou ingressou sessões ponto a ponto é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="d5ef1-132">Yammer</span><span class="sxs-lookup"><span data-stu-id="d5ef1-132">yammer</span></span>            | <span data-ttu-id="d5ef1-133">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ef1-133">Int64</span></span>  | <span data-ttu-id="d5ef1-134">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-134">The number of active users in Yammer.</span></span> <span data-ttu-id="d5ef1-135">Qualquer usuário que pode postar, ler ou like mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="d5ef1-136">equipes</span><span class="sxs-lookup"><span data-stu-id="d5ef1-136">teams</span></span>             | <span data-ttu-id="d5ef1-137">Int64</span><span class="sxs-lookup"><span data-stu-id="d5ef1-137">Int64</span></span>  | <span data-ttu-id="d5ef1-138">O número de usuários ativos em Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="d5ef1-139">Qualquer usuário que as mensagens postadas no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="d5ef1-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="d5ef1-140">reportDate</span></span>        | <span data-ttu-id="d5ef1-141">Data</span><span class="sxs-lookup"><span data-stu-id="d5ef1-141">Date</span></span>   | <span data-ttu-id="d5ef1-142">A data em que um número de usuários estava ativo.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="d5ef1-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d5ef1-143">reportPeriod</span></span>      | <span data-ttu-id="d5ef1-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d5ef1-144">String</span></span> | <span data-ttu-id="d5ef1-145">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d5ef1-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d5ef1-146">JSON representation</span></span>

<span data-ttu-id="d5ef1-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d5ef1-147">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "office365": 1024, 
  "exchange": 1024, 
  "oneDrive": 1024, 
  "sharePoint": 1024, 
  "skypeForBusiness": 1024, 
  "yammer": 1024, 
  "teams": 1024, 
  "reportDate": "Date", 
  "reportPeriod": "String"
}
```
