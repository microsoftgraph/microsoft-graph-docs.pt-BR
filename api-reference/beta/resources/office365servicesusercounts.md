---
title: tipo de recurso office365ServicesUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 5958ab3cb05767465b0866078d378208f1b466e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009465"
---
# <a name="office365servicesusercounts-resource-type"></a><span data-ttu-id="32b10-103">tipo de recurso office365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="32b10-103">office365ServicesUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="32b10-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32b10-104">Properties</span></span>

| <span data-ttu-id="32b10-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32b10-105">Property</span></span>                 | <span data-ttu-id="32b10-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="32b10-106">Type</span></span>   | <span data-ttu-id="32b10-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="32b10-107">Description</span></span>                              |
| :----------------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="32b10-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="32b10-108">reportRefreshDate</span></span>        | <span data-ttu-id="32b10-109">Data</span><span class="sxs-lookup"><span data-stu-id="32b10-109">Date</span></span>   | <span data-ttu-id="32b10-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="32b10-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="32b10-111">exchangeActive</span><span class="sxs-lookup"><span data-stu-id="32b10-111">exchangeActive</span></span>           | <span data-ttu-id="32b10-112">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-112">Int64</span></span>  | <span data-ttu-id="32b10-113">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="32b10-113">The number of active users on Exchange.</span></span> <span data-ttu-id="32b10-114">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="32b10-114">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="32b10-115">exchangeInactive</span><span class="sxs-lookup"><span data-stu-id="32b10-115">exchangeInactive</span></span>         | <span data-ttu-id="32b10-116">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-116">Int64</span></span>  | <span data-ttu-id="32b10-117">O número de usuários inativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="32b10-117">The number of inactive users on Exchange.</span></span> |
| <span data-ttu-id="32b10-118">oneDriveActive</span><span class="sxs-lookup"><span data-stu-id="32b10-118">oneDriveActive</span></span>           | <span data-ttu-id="32b10-119">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-119">Int64</span></span>  | <span data-ttu-id="32b10-120">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="32b10-120">The number of active users on OneDrive.</span></span> <span data-ttu-id="32b10-121">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="32b10-121">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="32b10-122">oneDriveInactive</span><span class="sxs-lookup"><span data-stu-id="32b10-122">oneDriveInactive</span></span>         | <span data-ttu-id="32b10-123">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-123">Int64</span></span>  | <span data-ttu-id="32b10-124">O número de usuários inativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="32b10-124">The number of inactive users on OneDrive.</span></span> |
| <span data-ttu-id="32b10-125">sharePointActive</span><span class="sxs-lookup"><span data-stu-id="32b10-125">sharePointActive</span></span>         | <span data-ttu-id="32b10-126">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-126">Int64</span></span>  | <span data-ttu-id="32b10-127">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="32b10-127">The number of active users on SharePoint.</span></span> <span data-ttu-id="32b10-128">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="32b10-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="32b10-129">sharePointInactive</span><span class="sxs-lookup"><span data-stu-id="32b10-129">sharePointInactive</span></span>       | <span data-ttu-id="32b10-130">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-130">Int64</span></span>  | <span data-ttu-id="32b10-131">O número de usuários inativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="32b10-131">The number of inactive users on SharePoint.</span></span> |
| <span data-ttu-id="32b10-132">skypeForBusinessActive</span><span class="sxs-lookup"><span data-stu-id="32b10-132">skypeForBusinessActive</span></span>   | <span data-ttu-id="32b10-133">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-133">Int64</span></span>  | <span data-ttu-id="32b10-134">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="32b10-134">The number of active users on Skype For Business.</span></span> <span data-ttu-id="32b10-135">Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="32b10-135">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="32b10-136">skypeForBusinessInactive</span><span class="sxs-lookup"><span data-stu-id="32b10-136">skypeForBusinessInactive</span></span> | <span data-ttu-id="32b10-137">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-137">Int64</span></span>  | <span data-ttu-id="32b10-138">O número de usuários inativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="32b10-138">The number of inactive users on Skype For Business.</span></span> |
| <span data-ttu-id="32b10-139">yammerActive</span><span class="sxs-lookup"><span data-stu-id="32b10-139">yammerActive</span></span>             | <span data-ttu-id="32b10-140">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-140">Int64</span></span>  | <span data-ttu-id="32b10-141">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="32b10-141">The number of active users on Yammer.</span></span> <span data-ttu-id="32b10-142">Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="32b10-142">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="32b10-143">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="32b10-143">yammerInactive</span></span>           | <span data-ttu-id="32b10-144">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-144">Int64</span></span>  | <span data-ttu-id="32b10-145">O número de usuários inativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="32b10-145">The number of inactive users on Yammer.</span></span>  |
| <span data-ttu-id="32b10-146">teamsActive</span><span class="sxs-lookup"><span data-stu-id="32b10-146">teamsActive</span></span>              | <span data-ttu-id="32b10-147">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-147">Int64</span></span>  | <span data-ttu-id="32b10-148">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="32b10-148">The number of active users on Microsoft Teams.</span></span> <span data-ttu-id="32b10-149">Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="32b10-149">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="32b10-150">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="32b10-150">teamsInactive</span></span>            | <span data-ttu-id="32b10-151">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-151">Int64</span></span>  | <span data-ttu-id="32b10-152">O número de usuários inativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="32b10-152">The number of inactive users on Microsoft Teams.</span></span>     |
| <span data-ttu-id="32b10-153">office365Active</span><span class="sxs-lookup"><span data-stu-id="32b10-153">office365Active</span></span>          | <span data-ttu-id="32b10-154">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-154">Int64</span></span>  | <span data-ttu-id="32b10-155">O número de usuários ativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="32b10-155">The number of active users on Office 365.</span></span>   |
| <span data-ttu-id="32b10-156">office365Inactive</span><span class="sxs-lookup"><span data-stu-id="32b10-156">office365Inactive</span></span>        | <span data-ttu-id="32b10-157">Int64</span><span class="sxs-lookup"><span data-stu-id="32b10-157">Int64</span></span>  | <span data-ttu-id="32b10-158">O número de usuários inativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="32b10-158">The number of inactive users on Office 365.</span></span>     |
| <span data-ttu-id="32b10-159">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="32b10-159">reportPeriod</span></span>             | <span data-ttu-id="32b10-160">String</span><span class="sxs-lookup"><span data-stu-id="32b10-160">String</span></span> | <span data-ttu-id="32b10-161">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="32b10-161">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="32b10-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32b10-162">JSON representation</span></span>

<span data-ttu-id="32b10-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32b10-163">The following is a JSON representation of the resource.</span></span>

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
