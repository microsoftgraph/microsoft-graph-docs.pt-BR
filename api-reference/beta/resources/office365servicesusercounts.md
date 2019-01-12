---
title: tipo de recurso de office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
ms.openlocfilehash: 54ae2020a5c02bba1469e3c6c0728024c72046bc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957301"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="463b9-103">tipo de recurso de office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="463b9-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="463b9-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="463b9-104">Properties</span></span>

| <span data-ttu-id="463b9-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="463b9-105">Property</span></span>                 | <span data-ttu-id="463b9-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="463b9-106">Type</span></span>   | <span data-ttu-id="463b9-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="463b9-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="463b9-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="463b9-108">reportRefreshDate</span></span>        | <span data-ttu-id="463b9-109">Data</span><span class="sxs-lookup"><span data-stu-id="463b9-109">Date</span></span>   | <span data-ttu-id="463b9-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="463b9-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="463b9-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="463b9-111">exchangeActive</span></span>           | <span data-ttu-id="463b9-112">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-112">Int64</span></span>  | <span data-ttu-id="463b9-113">O número de usuários ativos em Exchange.</span><span class="sxs-lookup"><span data-stu-id="463b9-113">The number of active users on Exchange.</span></span> <span data-ttu-id="463b9-114">Qualquer usuário que pode ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="463b9-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="463b9-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="463b9-115">exchangeInactive</span></span>         | <span data-ttu-id="463b9-116">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-116">Int64</span></span>  | <span data-ttu-id="463b9-117">O número de usuários inativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="463b9-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="463b9-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="463b9-118">oneDriveActive</span></span>           | <span data-ttu-id="463b9-119">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-119">Int64</span></span>  | <span data-ttu-id="463b9-120">O número de usuários ativos em OneDrive.</span><span class="sxs-lookup"><span data-stu-id="463b9-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="463b9-121">Qualquer usuário que são exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="463b9-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="463b9-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="463b9-122">oneDriveInactive</span></span>         | <span data-ttu-id="463b9-123">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-123">Int64</span></span>  | <span data-ttu-id="463b9-124">O número de usuários inativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="463b9-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="463b9-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="463b9-125">sharePointActive</span></span>         | <span data-ttu-id="463b9-126">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-126">Int64</span></span>  | <span data-ttu-id="463b9-127">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="463b9-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="463b9-128">Qualquer usuário que exibidos ou editados arquivos, internamente de arquivos compartilhados ou sincronizados arquivos externamente ou exibidos páginas do SharePoint é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="463b9-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="463b9-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="463b9-129">sharePointInactive</span></span>       | <span data-ttu-id="463b9-130">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-130">Int64</span></span>  | <span data-ttu-id="463b9-131">O número de usuários inativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="463b9-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="463b9-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="463b9-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="463b9-133">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-133">Int64</span></span>  | <span data-ttu-id="463b9-134">O número de usuários ativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="463b9-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="463b9-135">Qualquer usuário que organizou participou de conferências ou ingressou sessões ponto a ponto é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="463b9-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="463b9-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="463b9-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="463b9-137">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-137">Int64</span></span>  | <span data-ttu-id="463b9-138">O número de usuários inativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="463b9-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="463b9-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="463b9-139">yammerActive</span></span>             | <span data-ttu-id="463b9-140">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-140">Int64</span></span>  | <span data-ttu-id="463b9-141">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="463b9-141">The number of active users on Yammer.</span></span> <span data-ttu-id="463b9-142">Qualquer usuário que pode postar, ler ou like mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="463b9-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="463b9-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="463b9-143">yammerInactive</span></span>           | <span data-ttu-id="463b9-144">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-144">Int64</span></span>  | <span data-ttu-id="463b9-145">O número de usuários inativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="463b9-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="463b9-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="463b9-146">teamsActive</span></span>              | <span data-ttu-id="463b9-147">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-147">Int64</span></span>  | <span data-ttu-id="463b9-148">O número de usuários ativos em equipes.</span><span class="sxs-lookup"><span data-stu-id="463b9-148">The number of active users on Teams.</span></span> <span data-ttu-id="463b9-149">Qualquer usuário que as mensagens postadas no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="463b9-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="463b9-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="463b9-150">teamsInactive</span></span>            | <span data-ttu-id="463b9-151">Int64</span><span class="sxs-lookup"><span data-stu-id="463b9-151">Int64</span></span>  | <span data-ttu-id="463b9-152">O número de usuários ativos em equipes.</span><span class="sxs-lookup"><span data-stu-id="463b9-152">The number of active users on Teams.</span></span>     |
| <span data-ttu-id="463b9-153">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="463b9-153">reportPeriod</span></span>             | <span data-ttu-id="463b9-154">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="463b9-154">String</span></span> | <span data-ttu-id="463b9-155">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="463b9-155">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="463b9-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="463b9-156">JSON representation</span></span>

<span data-ttu-id="463b9-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="463b9-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "exchangeActive": 1024, 
  "exchangeInactive": 1024, 
  "oneDriveActive": 1024, 
  "oneDriveInactive": 1024, 
  "sharePointActive": 1024, 
  "sharePointInactive": 1024, 
  "skypeForBusinessActive": 1024, 
  "skypeForBusinessInactive": 1024, 
  "yammerActive": 1024, 
  "yammerInactive": 1024, 
  "teamsActive": 1024, 
  "teamsInactive": 1024, 
  "reportPeriod": "String"
}
```
