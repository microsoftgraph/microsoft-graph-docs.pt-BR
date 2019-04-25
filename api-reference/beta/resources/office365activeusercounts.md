---
title: tipo de recurso office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bbc51e4859b005c01b0f8d2cfb2db3ca902d60e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32581454"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="a9056-103">tipo de recurso office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="a9056-103">office365ActiveUserCounts resource type</span></span>

## <a name="properties"></a><span data-ttu-id="a9056-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a9056-104">Properties</span></span>

| <span data-ttu-id="a9056-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a9056-105">Property</span></span>          | <span data-ttu-id="a9056-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="a9056-106">Type</span></span>   | <span data-ttu-id="a9056-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="a9056-107">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="a9056-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a9056-108">reportRefreshDate</span></span> | <span data-ttu-id="a9056-109">Data</span><span class="sxs-lookup"><span data-stu-id="a9056-109">Date</span></span>   | <span data-ttu-id="a9056-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a9056-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="a9056-111">Office365</span><span class="sxs-lookup"><span data-stu-id="a9056-111">office365</span></span>         | <span data-ttu-id="a9056-112">Int64</span><span class="sxs-lookup"><span data-stu-id="a9056-112">Int64</span></span>  | <span data-ttu-id="a9056-113">O número de usuários ativos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="a9056-113">The number of active users in Office 365.</span></span> <span data-ttu-id="a9056-114">Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype for Business, Yammer e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a9056-114">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="a9056-115">Você pode encontrar a definição de usuário ativo para cada produto na respectiva descrição da propriedade.</span><span class="sxs-lookup"><span data-stu-id="a9056-115">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="a9056-116">câmbio</span><span class="sxs-lookup"><span data-stu-id="a9056-116">exchange</span></span>          | <span data-ttu-id="a9056-117">Int64</span><span class="sxs-lookup"><span data-stu-id="a9056-117">Int64</span></span>  | <span data-ttu-id="a9056-118">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9056-118">The number of active users in Exchange.</span></span> <span data-ttu-id="a9056-119">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="a9056-119">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="a9056-120">oneDrive</span><span class="sxs-lookup"><span data-stu-id="a9056-120">oneDrive</span></span>          | <span data-ttu-id="a9056-121">Int64</span><span class="sxs-lookup"><span data-stu-id="a9056-121">Int64</span></span>  | <span data-ttu-id="a9056-122">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a9056-122">The number of active users in OneDrive.</span></span> <span data-ttu-id="a9056-123">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="a9056-123">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="a9056-124">Do</span><span class="sxs-lookup"><span data-stu-id="a9056-124">sharePoint</span></span>        | <span data-ttu-id="a9056-125">Int64</span><span class="sxs-lookup"><span data-stu-id="a9056-125">Int64</span></span>  | <span data-ttu-id="a9056-126">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a9056-126">The number of active users in SharePoint.</span></span> <span data-ttu-id="a9056-127">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="a9056-127">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="a9056-128">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="a9056-128">skypeForBusiness</span></span>  | <span data-ttu-id="a9056-129">Int64</span><span class="sxs-lookup"><span data-stu-id="a9056-129">Int64</span></span>  | <span data-ttu-id="a9056-130">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="a9056-130">The number of active users in Skype For Business.</span></span> <span data-ttu-id="a9056-131">Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="a9056-131">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="a9056-132">Yammer</span><span class="sxs-lookup"><span data-stu-id="a9056-132">yammer</span></span>            | <span data-ttu-id="a9056-133">Int64</span><span class="sxs-lookup"><span data-stu-id="a9056-133">Int64</span></span>  | <span data-ttu-id="a9056-134">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a9056-134">The number of active users in Yammer.</span></span> <span data-ttu-id="a9056-135">Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="a9056-135">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="a9056-136">Teams</span><span class="sxs-lookup"><span data-stu-id="a9056-136">teams</span></span>             | <span data-ttu-id="a9056-137">Int64</span><span class="sxs-lookup"><span data-stu-id="a9056-137">Int64</span></span>  | <span data-ttu-id="a9056-138">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a9056-138">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="a9056-139">Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="a9056-139">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="a9056-140">reportDate</span><span class="sxs-lookup"><span data-stu-id="a9056-140">reportDate</span></span>        | <span data-ttu-id="a9056-141">Data</span><span class="sxs-lookup"><span data-stu-id="a9056-141">Date</span></span>   | <span data-ttu-id="a9056-142">A data em que um número de usuários estava ativo.</span><span class="sxs-lookup"><span data-stu-id="a9056-142">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="a9056-143">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a9056-143">reportPeriod</span></span>      | <span data-ttu-id="a9056-144">String</span><span class="sxs-lookup"><span data-stu-id="a9056-144">String</span></span> | <span data-ttu-id="a9056-145">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="a9056-145">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="a9056-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a9056-146">JSON representation</span></span>

<span data-ttu-id="a9056-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a9056-147">The following is a JSON representation of the resource.</span></span>

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
