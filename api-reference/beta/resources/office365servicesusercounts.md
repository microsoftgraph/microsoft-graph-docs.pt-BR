---
title: tipo de recurso de office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 975a70b040ac5886ea36219a5407f580a42aeadc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034071"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="d0c36-103">tipo de recurso de office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="d0c36-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="d0c36-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0c36-104">Properties</span></span>

| <span data-ttu-id="d0c36-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0c36-105">Property</span></span>                 | <span data-ttu-id="d0c36-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0c36-106">Type</span></span>   | <span data-ttu-id="d0c36-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0c36-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="d0c36-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="d0c36-108">reportRefreshDate</span></span>        | <span data-ttu-id="d0c36-109">Data</span><span class="sxs-lookup"><span data-stu-id="d0c36-109">Date</span></span>   | <span data-ttu-id="d0c36-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="d0c36-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="d0c36-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="d0c36-111">exchangeActive</span></span>           | <span data-ttu-id="d0c36-112">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-112">Int64</span></span>  | <span data-ttu-id="d0c36-113">O número de usuários ativos em Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0c36-113">The number of active users on Exchange.</span></span> <span data-ttu-id="d0c36-114">Qualquer usuário que pode ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d0c36-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="d0c36-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="d0c36-115">exchangeInactive</span></span>         | <span data-ttu-id="d0c36-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-116">Int64</span></span>  | <span data-ttu-id="d0c36-117">O número de usuários inativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0c36-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="d0c36-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="d0c36-118">oneDriveActive</span></span>           | <span data-ttu-id="d0c36-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-119">Int64</span></span>  | <span data-ttu-id="d0c36-120">O número de usuários ativos em OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d0c36-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="d0c36-121">Qualquer usuário que são exibidos ou editados arquivos, arquivos compartilhados interna ou externamente ou sincronizados arquivos é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d0c36-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="d0c36-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="d0c36-122">oneDriveInactive</span></span>         | <span data-ttu-id="d0c36-123">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-123">Int64</span></span>  | <span data-ttu-id="d0c36-124">O número de usuários inativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d0c36-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="d0c36-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="d0c36-125">sharePointActive</span></span>         | <span data-ttu-id="d0c36-126">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-126">Int64</span></span>  | <span data-ttu-id="d0c36-127">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d0c36-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="d0c36-128">Qualquer usuário que exibidos ou editados arquivos, internamente de arquivos compartilhados ou sincronizados arquivos externamente ou exibidos páginas do SharePoint é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d0c36-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="d0c36-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="d0c36-129">sharePointInactive</span></span>       | <span data-ttu-id="d0c36-130">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-130">Int64</span></span>  | <span data-ttu-id="d0c36-131">O número de usuários inativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="d0c36-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="d0c36-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="d0c36-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="d0c36-133">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-133">Int64</span></span>  | <span data-ttu-id="d0c36-134">O número de usuários ativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="d0c36-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="d0c36-135">Qualquer usuário que organizou participou de conferências ou ingressou sessões ponto a ponto é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d0c36-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="d0c36-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="d0c36-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="d0c36-137">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-137">Int64</span></span>  | <span data-ttu-id="d0c36-138">O número de usuários inativos em Skype para negócios.</span><span class="sxs-lookup"><span data-stu-id="d0c36-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="d0c36-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="d0c36-139">yammerActive</span></span>             | <span data-ttu-id="d0c36-140">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-140">Int64</span></span>  | <span data-ttu-id="d0c36-141">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="d0c36-141">The number of active users on Yammer.</span></span> <span data-ttu-id="d0c36-142">Qualquer usuário que pode postar, ler ou like mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d0c36-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="d0c36-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="d0c36-143">yammerInactive</span></span>           | <span data-ttu-id="d0c36-144">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-144">Int64</span></span>  | <span data-ttu-id="d0c36-145">O número de usuários inativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="d0c36-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="d0c36-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="d0c36-146">teamsActive</span></span>              | <span data-ttu-id="d0c36-147">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-147">Int64</span></span>  | <span data-ttu-id="d0c36-148">O número de usuários ativos em equipes.</span><span class="sxs-lookup"><span data-stu-id="d0c36-148">The number of active users on Teams.</span></span> <span data-ttu-id="d0c36-149">Qualquer usuário que as mensagens postadas no canais de equipe, mensagens enviadas em sessões de bate-papo privado ou participou chamadas ou reuniões é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="d0c36-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="d0c36-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="d0c36-150">teamsInactive</span></span>            | <span data-ttu-id="d0c36-151">Int64</span><span class="sxs-lookup"><span data-stu-id="d0c36-151">Int64</span></span>  | <span data-ttu-id="d0c36-152">O número de usuários ativos em equipes.</span><span class="sxs-lookup"><span data-stu-id="d0c36-152">The number of active users on Teams.</span></span>     |
| <span data-ttu-id="d0c36-153">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="d0c36-153">reportPeriod</span></span>             | <span data-ttu-id="d0c36-154">String</span><span class="sxs-lookup"><span data-stu-id="d0c36-154">String</span></span> | <span data-ttu-id="d0c36-155">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="d0c36-155">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="d0c36-156">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0c36-156">JSON representation</span></span>

<span data-ttu-id="d0c36-157">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0c36-157">The following is a JSON representation of the resource.</span></span>

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
