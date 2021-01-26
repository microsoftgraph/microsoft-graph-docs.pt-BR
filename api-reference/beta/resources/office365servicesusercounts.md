---
title: Tipo de recurso office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: 276153f9613f464cdf11f6dfdad307bb341f646d
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982149"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="80403-103">Tipo de recurso office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="80403-103">office365ServicesUserCounts resource type</span></span>

<span data-ttu-id="80403-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80403-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="80403-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="80403-105">Properties</span></span>

| <span data-ttu-id="80403-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80403-106">Property</span></span>                 | <span data-ttu-id="80403-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="80403-107">Type</span></span>   | <span data-ttu-id="80403-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="80403-108">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="80403-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="80403-109">reportRefreshDate</span></span>        | <span data-ttu-id="80403-110">Data</span><span class="sxs-lookup"><span data-stu-id="80403-110">Date</span></span>   | <span data-ttu-id="80403-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="80403-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="80403-112">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="80403-112">exchangeActive</span></span>           | <span data-ttu-id="80403-113">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-113">Int64</span></span>  | <span data-ttu-id="80403-114">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="80403-114">The number of active users on Exchange.</span></span> <span data-ttu-id="80403-115">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="80403-115">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="80403-116">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="80403-116">exchangeInactive</span></span>         | <span data-ttu-id="80403-117">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-117">Int64</span></span>  | <span data-ttu-id="80403-118">O número de usuários inativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="80403-118">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="80403-119">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="80403-119">oneDriveActive</span></span>           | <span data-ttu-id="80403-120">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-120">Int64</span></span>  | <span data-ttu-id="80403-121">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="80403-121">The number of active users on OneDrive.</span></span> <span data-ttu-id="80403-122">Qualquer usuário que visualizou ou editou arquivos, compartilhou arquivos interna ou externamente ou arquivos sincronizados é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="80403-122">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="80403-123">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="80403-123">oneDriveInactive</span></span>         | <span data-ttu-id="80403-124">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-124">Int64</span></span>  | <span data-ttu-id="80403-125">O número de usuários inativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="80403-125">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="80403-126">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="80403-126">sharePointActive</span></span>         | <span data-ttu-id="80403-127">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-127">Int64</span></span>  | <span data-ttu-id="80403-128">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="80403-128">The number of active users on SharePoint.</span></span> <span data-ttu-id="80403-129">Qualquer usuário que visualizou ou editou arquivos, compartilhou arquivos interna ou externamente, sincronizou arquivos ou visualizou páginas do SharePoint é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="80403-129">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="80403-130">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="80403-130">sharePointInactive</span></span>       | <span data-ttu-id="80403-131">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-131">Int64</span></span>  | <span data-ttu-id="80403-132">O número de usuários inativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="80403-132">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="80403-133">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="80403-133">skypeForBusinessActive</span></span>   | <span data-ttu-id="80403-134">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-134">Int64</span></span>  | <span data-ttu-id="80403-135">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="80403-135">The number of active users on Skype For Business.</span></span> <span data-ttu-id="80403-136">Qualquer usuário que organizou ou participou de conferências ou ingressou em sessões ponto a ponto é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="80403-136">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="80403-137">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="80403-137">skypeForBusinessInactive</span></span> | <span data-ttu-id="80403-138">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-138">Int64</span></span>  | <span data-ttu-id="80403-139">O número de usuários inativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="80403-139">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="80403-140">yammerActive</span><span class="sxs-lookup"><span data-stu-id="80403-140">yammerActive</span></span>             | <span data-ttu-id="80403-141">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-141">Int64</span></span>  | <span data-ttu-id="80403-142">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="80403-142">The number of active users on Yammer.</span></span> <span data-ttu-id="80403-143">Qualquer usuário que possa postar, ler ou como mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="80403-143">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="80403-144">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="80403-144">yammerInactive</span></span>           | <span data-ttu-id="80403-145">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-145">Int64</span></span>  | <span data-ttu-id="80403-146">O número de usuários inativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="80403-146">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="80403-147">teamsActive</span><span class="sxs-lookup"><span data-stu-id="80403-147">teamsActive</span></span>              | <span data-ttu-id="80403-148">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-148">Int64</span></span>  | <span data-ttu-id="80403-149">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="80403-149">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="80403-150">Qualquer usuário que postou mensagens em canais de equipe, enviou mensagens em sessões de chat privado ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="80403-150">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="80403-151">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="80403-151">teamsInactive</span></span>            | <span data-ttu-id="80403-152">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-152">Int64</span></span>  | <span data-ttu-id="80403-153">O número de usuários inativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="80403-153">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="80403-154">office365Active</span><span class="sxs-lookup"><span data-stu-id="80403-154">office365Active</span></span>          | <span data-ttu-id="80403-155">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-155">Int64</span></span>  | <span data-ttu-id="80403-156">O número de usuários ativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="80403-156">The number of active users on Microsoft 365.</span></span>   |
| <span data-ttu-id="80403-157">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="80403-157">office365Inactive</span></span>        | <span data-ttu-id="80403-158">Int64</span><span class="sxs-lookup"><span data-stu-id="80403-158">Int64</span></span>  | <span data-ttu-id="80403-159">O número de usuários inativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="80403-159">The number of inactive users on Microsoft 365.</span></span>     |
| <span data-ttu-id="80403-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="80403-160">reportPeriod</span></span>             | <span data-ttu-id="80403-161">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80403-161">String</span></span> | <span data-ttu-id="80403-162">O número de dias que o relatório abrange.</span><span class="sxs-lookup"><span data-stu-id="80403-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="80403-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="80403-163">JSON representation</span></span>

<span data-ttu-id="80403-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="80403-164">The following is a JSON representation of the resource.</span></span>

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
  "office365Active": 1024,
  "office365Inactive": 1024,
  "reportPeriod": "String"
}
```


