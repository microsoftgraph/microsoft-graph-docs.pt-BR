---
title: tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: b7e22c522bf6cffeba6f09c350abaaabeda23b1b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092409"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="a1335-103">tipo de recurso office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="a1335-103">office365GroupsActivityDetail resource type</span></span>

<span data-ttu-id="a1335-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1335-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="a1335-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1335-105">Properties</span></span>

| <span data-ttu-id="a1335-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1335-106">Property</span></span>                          | <span data-ttu-id="a1335-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1335-107">Type</span></span>    | <span data-ttu-id="a1335-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1335-108">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="a1335-109">groupId</span><span class="sxs-lookup"><span data-stu-id="a1335-109">groupId</span></span>                           | <span data-ttu-id="a1335-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1335-110">String</span></span>  | <span data-ttu-id="a1335-111">A ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-111">The group id.</span></span>          |
| <span data-ttu-id="a1335-112">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="a1335-112">reportRefreshDate</span></span>                 | <span data-ttu-id="a1335-113">Data</span><span class="sxs-lookup"><span data-stu-id="a1335-113">Date</span></span>    | <span data-ttu-id="a1335-114">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a1335-114">The latest date of the content.</span></span>          |
| <span data-ttu-id="a1335-115">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="a1335-115">groupDisplayName</span></span>                  | <span data-ttu-id="a1335-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1335-116">String</span></span>  | <span data-ttu-id="a1335-117">O nome de exibição do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-117">The display name of the group.</span></span>           |
| <span data-ttu-id="a1335-118">isDeleted</span><span class="sxs-lookup"><span data-stu-id="a1335-118">isDeleted</span></span>                         | <span data-ttu-id="a1335-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1335-119">Boolean</span></span> | <span data-ttu-id="a1335-120">Se este usuário foi excluído ou excluído por software.</span><span class="sxs-lookup"><span data-stu-id="a1335-120">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="a1335-121">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a1335-121">ownerPrincipalName</span></span>                | <span data-ttu-id="a1335-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1335-122">String</span></span>  | <span data-ttu-id="a1335-123">O nome principal do proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-123">The group owner principal name.</span></span>          |
| <span data-ttu-id="a1335-124">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="a1335-124">lastActivityDate</span></span>                  | <span data-ttu-id="a1335-125">Data</span><span class="sxs-lookup"><span data-stu-id="a1335-125">Date</span></span>    | <span data-ttu-id="a1335-126">A data da última atividade dos seguintes cenários: caixa de correio de grupo recebidas emails; arquivos de usuário exibidos, editados, compartilhados ou sincronizados na biblioteca de documentos do SharePoint; páginas do SharePoint exibidas pelo usuário; mensagens postadas, lidas ou curtidas pelo usuário em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1335-126">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="a1335-127">groupType</span><span class="sxs-lookup"><span data-stu-id="a1335-127">groupType</span></span>                         | <span data-ttu-id="a1335-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1335-128">String</span></span>  | <span data-ttu-id="a1335-129">O tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-129">The group type.</span></span> <span data-ttu-id="a1335-130">Os valores possíveis são: **Public** ou **Private**.</span><span class="sxs-lookup"><span data-stu-id="a1335-130">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="a1335-131">memberCount</span><span class="sxs-lookup"><span data-stu-id="a1335-131">memberCount</span></span>                       | <span data-ttu-id="a1335-132">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-132">Int64</span></span>   | <span data-ttu-id="a1335-133">A contagem de membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-133">The group member count.</span></span>                  |
| <span data-ttu-id="a1335-134">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="a1335-134">externalMemberCount</span></span>               | <span data-ttu-id="a1335-135">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-135">Int64</span></span>   | <span data-ttu-id="a1335-136">A contagem de membros externos de grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-136">The group external member count.</span></span>         |
| <span data-ttu-id="a1335-137">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="a1335-137">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="a1335-138">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-138">Int64</span></span>   | <span data-ttu-id="a1335-139">O número de emails que a caixa de correio de grupo recebeu.</span><span class="sxs-lookup"><span data-stu-id="a1335-139">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="a1335-140">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="a1335-140">sharePointActiveFileCount</span></span>         | <span data-ttu-id="a1335-141">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-141">Int64</span></span>   | <span data-ttu-id="a1335-142">O número de arquivos ativos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a1335-142">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="a1335-143">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="a1335-143">yammerPostedMessageCount</span></span>          | <span data-ttu-id="a1335-144">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-144">Int64</span></span>   | <span data-ttu-id="a1335-145">O número de mensagens postadas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1335-145">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="a1335-146">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="a1335-146">yammerReadMessageCount</span></span>            | <span data-ttu-id="a1335-147">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-147">Int64</span></span>   | <span data-ttu-id="a1335-148">O número de mensagens lidas nos grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1335-148">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="a1335-149">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="a1335-149">yammerLikedMessageCount</span></span>           | <span data-ttu-id="a1335-150">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-150">Int64</span></span>   | <span data-ttu-id="a1335-151">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1335-151">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="a1335-152">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="a1335-152">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="a1335-153">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-153">Int64</span></span>   | <span data-ttu-id="a1335-154">O número de itens na caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-154">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="a1335-155">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="a1335-155">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="a1335-156">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-156">Int64</span></span>   | <span data-ttu-id="a1335-157">O armazenamento usado da caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="a1335-157">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="a1335-158">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="a1335-158">sharePointTotalFileCount</span></span>          | <span data-ttu-id="a1335-159">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-159">Int64</span></span>   | <span data-ttu-id="a1335-160">O número total de arquivos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a1335-160">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="a1335-161">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="a1335-161">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="a1335-162">Int64</span><span class="sxs-lookup"><span data-stu-id="a1335-162">Int64</span></span>   | <span data-ttu-id="a1335-163">O armazenamento usado pelo site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a1335-163">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="a1335-164">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="a1335-164">reportPeriod</span></span>                      | <span data-ttu-id="a1335-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a1335-165">String</span></span>  | <span data-ttu-id="a1335-166">O número de dias que o relatório cobre.</span><span class="sxs-lookup"><span data-stu-id="a1335-166">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="a1335-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1335-167">JSON representation</span></span>

<span data-ttu-id="a1335-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1335-168">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
  "groupId": "0003cf63-7ff3-4471-b24b-50ffbfb8b5d2",
  "reportRefreshDate": "Date", 
  "groupDisplayName": "String", 
  "isDeleted": true, 
  "ownerPrincipalName": "String", 
  "lastActivityDate": "Date", 
  "groupType": "String", 
  "memberCount": 1024, 
  "externalMemberCount": 1024, 
  "exchangeReceivedEmailCount": 1024, 
  "sharePointActiveFileCount": 1024, 
  "yammerPostedMessageCount": 1024, 
  "yammerReadMessageCount": 1024, 
  "yammerLikedMessageCount": 1024, 
  "exchangeMailboxTotalItemCount": 1024, 
  "exchangeMailboxStorageUsedInBytes": 1024, 
  "sharePointTotalFileCount": 1024, 
  "sharePointSiteStorageUsedInBytes": 1024, 
  "reportPeriod": "String"
}
```


