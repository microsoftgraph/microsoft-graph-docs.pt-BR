---
title: tipo de recurso office365ActiveUserCounts
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 8d640bbb3f49c95902134893f1eba4b4064ccca5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092451"
---
# <a name="office365activeusercounts-resource-type"></a><span data-ttu-id="5c50c-103">tipo de recurso office365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="5c50c-103">office365ActiveUserCounts resource type</span></span>

<span data-ttu-id="5c50c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c50c-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="5c50c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c50c-105">Properties</span></span>

| <span data-ttu-id="5c50c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c50c-106">Property</span></span>          | <span data-ttu-id="5c50c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c50c-107">Type</span></span>   | <span data-ttu-id="5c50c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c50c-108">Description</span></span>                              |
| :---------------- | :----- | ---------------------------------------- |
| <span data-ttu-id="5c50c-109">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="5c50c-109">reportRefreshDate</span></span> | <span data-ttu-id="5c50c-110">Data</span><span class="sxs-lookup"><span data-stu-id="5c50c-110">Date</span></span>   | <span data-ttu-id="5c50c-111">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-111">The latest date of the content.</span></span>          |
| <span data-ttu-id="5c50c-112">Office365</span><span class="sxs-lookup"><span data-stu-id="5c50c-112">office365</span></span>         | <span data-ttu-id="5c50c-113">Int64</span><span class="sxs-lookup"><span data-stu-id="5c50c-113">Int64</span></span>  | <span data-ttu-id="5c50c-114">O número de usuários ativos no Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5c50c-114">The number of active users in Microsoft 365.</span></span> <span data-ttu-id="5c50c-115">Esse número inclui todos os usuários ativos no Exchange, OneDrive, SharePoint, Skype for Business, Yammer e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5c50c-115">This number includes all the active users in Exchange, OneDrive, SharePoint, Skype For Business, Yammer, and Microsoft Teams.</span></span> <span data-ttu-id="5c50c-116">Você pode encontrar a definição de usuário ativo para cada produto na respectiva descrição da propriedade.</span><span class="sxs-lookup"><span data-stu-id="5c50c-116">You can find the definition of active user for each product in the respective property description.</span></span> |
| <span data-ttu-id="5c50c-117">câmbio</span><span class="sxs-lookup"><span data-stu-id="5c50c-117">exchange</span></span>          | <span data-ttu-id="5c50c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="5c50c-118">Int64</span></span>  | <span data-ttu-id="5c50c-119">O número de usuários ativos no Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c50c-119">The number of active users in Exchange.</span></span> <span data-ttu-id="5c50c-120">Qualquer usuário que possa ler e enviar emails é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-120">Any user who can read and send email is considered an active user.</span></span> |
| <span data-ttu-id="5c50c-121">oneDrive</span><span class="sxs-lookup"><span data-stu-id="5c50c-121">oneDrive</span></span>          | <span data-ttu-id="5c50c-122">Int64</span><span class="sxs-lookup"><span data-stu-id="5c50c-122">Int64</span></span>  | <span data-ttu-id="5c50c-123">O número de usuários ativos no OneDrive.</span><span class="sxs-lookup"><span data-stu-id="5c50c-123">The number of active users in OneDrive.</span></span> <span data-ttu-id="5c50c-124">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, ou arquivos sincronizados é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-124">Any user who viewed or edited files, shared files internally or externally, or synced files is considered an active user.</span></span> |
| <span data-ttu-id="5c50c-125">Do</span><span class="sxs-lookup"><span data-stu-id="5c50c-125">sharePoint</span></span>        | <span data-ttu-id="5c50c-126">Int64</span><span class="sxs-lookup"><span data-stu-id="5c50c-126">Int64</span></span>  | <span data-ttu-id="5c50c-127">O número de usuários ativos no SharePoint.</span><span class="sxs-lookup"><span data-stu-id="5c50c-127">The number of active users in SharePoint.</span></span> <span data-ttu-id="5c50c-128">Qualquer usuário que tenha exibido ou editado arquivos, arquivos compartilhados internamente ou externamente, arquivos sincronizados ou páginas do SharePoint exibidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-128">Any user who viewed or edited files, shared files internally or externally, synced files, or viewed SharePoint pages is considered an active user.</span></span> |
| <span data-ttu-id="5c50c-129">skypeForBusiness</span><span class="sxs-lookup"><span data-stu-id="5c50c-129">skypeForBusiness</span></span>  | <span data-ttu-id="5c50c-130">Int64</span><span class="sxs-lookup"><span data-stu-id="5c50c-130">Int64</span></span>  | <span data-ttu-id="5c50c-131">O número de usuários ativos no Skype for Business.</span><span class="sxs-lookup"><span data-stu-id="5c50c-131">The number of active users in Skype For Business.</span></span> <span data-ttu-id="5c50c-132">Qualquer usuário que organizou ou participou de conferências ou sessões ponto a ponto Unidas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-132">Any user who organized or participated in conferences, or joined peer-to-peer sessions is considered an active user.</span></span> |
| <span data-ttu-id="5c50c-133">Yammer</span><span class="sxs-lookup"><span data-stu-id="5c50c-133">yammer</span></span>            | <span data-ttu-id="5c50c-134">Int64</span><span class="sxs-lookup"><span data-stu-id="5c50c-134">Int64</span></span>  | <span data-ttu-id="5c50c-135">O número de usuários ativos no Yammer.</span><span class="sxs-lookup"><span data-stu-id="5c50c-135">The number of active users in Yammer.</span></span> <span data-ttu-id="5c50c-136">Qualquer usuário que possa postar, ler ou gostar de mensagens é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-136">Any user who can post, read, or like messages is considered an active user.</span></span> |
| <span data-ttu-id="5c50c-137">Teams</span><span class="sxs-lookup"><span data-stu-id="5c50c-137">teams</span></span>             | <span data-ttu-id="5c50c-138">Int64</span><span class="sxs-lookup"><span data-stu-id="5c50c-138">Int64</span></span>  | <span data-ttu-id="5c50c-139">O número de usuários ativos no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="5c50c-139">The number of active users in Microsoft Teams.</span></span> <span data-ttu-id="5c50c-140">Qualquer usuário que lançou mensagens em canais de equipe, mensagens enviadas em sessões de chat privadas ou participou de reuniões ou chamadas é considerado um usuário ativo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-140">Any user who posted messages in team channels, sent messages in private chat sessions, or participated in meetings or calls is considered an active user.</span></span> |
| <span data-ttu-id="5c50c-141">reportDate</span><span class="sxs-lookup"><span data-stu-id="5c50c-141">reportDate</span></span>        | <span data-ttu-id="5c50c-142">Data</span><span class="sxs-lookup"><span data-stu-id="5c50c-142">Date</span></span>   | <span data-ttu-id="5c50c-143">A data em que um número de usuários estava ativo.</span><span class="sxs-lookup"><span data-stu-id="5c50c-143">The date on which a number of users were active.</span></span> |
| <span data-ttu-id="5c50c-144">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="5c50c-144">reportPeriod</span></span>      | <span data-ttu-id="5c50c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5c50c-145">String</span></span> | <span data-ttu-id="5c50c-146">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="5c50c-146">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="5c50c-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c50c-147">JSON representation</span></span>

<span data-ttu-id="5c50c-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c50c-148">The following is a JSON representation of the resource.</span></span>

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


