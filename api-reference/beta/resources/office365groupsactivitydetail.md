---
title: Tipo de recurso office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: fe2df5614525f27b294bed93be7f3f9cd8170b30
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981505"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="8d896-103">Tipo de recurso office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="8d896-103">office365GroupsActivityDetail resource type</span></span>

<span data-ttu-id="8d896-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d896-104">Namespace: microsoft.graph</span></span>

## <a name="properties"></a><span data-ttu-id="8d896-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8d896-105">Properties</span></span>

| <span data-ttu-id="8d896-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8d896-106">Property</span></span>                          | <span data-ttu-id="8d896-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8d896-107">Type</span></span>    | <span data-ttu-id="8d896-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8d896-108">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="8d896-109">groupId</span><span class="sxs-lookup"><span data-stu-id="8d896-109">groupId</span></span>                           | <span data-ttu-id="8d896-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d896-110">String</span></span>  | <span data-ttu-id="8d896-111">A ID do grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-111">The group id.</span></span>          |
| <span data-ttu-id="8d896-112">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="8d896-112">reportRefreshDate</span></span>                 | <span data-ttu-id="8d896-113">Data</span><span class="sxs-lookup"><span data-stu-id="8d896-113">Date</span></span>    | <span data-ttu-id="8d896-114">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="8d896-114">The latest date of the content.</span></span>          |
| <span data-ttu-id="8d896-115">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="8d896-115">groupDisplayName</span></span>                  | <span data-ttu-id="8d896-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d896-116">String</span></span>  | <span data-ttu-id="8d896-117">O nome de exibição do grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-117">The display name of the group.</span></span>           |
| <span data-ttu-id="8d896-118">isDeleted</span><span class="sxs-lookup"><span data-stu-id="8d896-118">isDeleted</span></span>                         | <span data-ttu-id="8d896-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="8d896-119">Boolean</span></span> | <span data-ttu-id="8d896-120">Se esse usuário foi excluído ou excluído de forma suave.</span><span class="sxs-lookup"><span data-stu-id="8d896-120">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="8d896-121">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8d896-121">ownerPrincipalName</span></span>                | <span data-ttu-id="8d896-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d896-122">String</span></span>  | <span data-ttu-id="8d896-123">O nome principal do proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-123">The group owner principal name.</span></span>          |
| <span data-ttu-id="8d896-124">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="8d896-124">lastActivityDate</span></span>                  | <span data-ttu-id="8d896-125">Data</span><span class="sxs-lookup"><span data-stu-id="8d896-125">Date</span></span>    | <span data-ttu-id="8d896-126">A data da última atividade para os seguintes cenários: caixa de correio de grupo recebeu emails; usuário visualizado, editado, compartilhado ou sincronizado arquivos na biblioteca de documentos do SharePoint; usuário visualizou páginas do SharePoint; usuário postou, leu ou curtiu mensagens em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d896-126">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="8d896-127">groupType</span><span class="sxs-lookup"><span data-stu-id="8d896-127">groupType</span></span>                         | <span data-ttu-id="8d896-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d896-128">String</span></span>  | <span data-ttu-id="8d896-129">O tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-129">The group type.</span></span> <span data-ttu-id="8d896-130">Os valores possíveis são: **Public** ou **Private**.</span><span class="sxs-lookup"><span data-stu-id="8d896-130">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="8d896-131">memberCount</span><span class="sxs-lookup"><span data-stu-id="8d896-131">memberCount</span></span>                       | <span data-ttu-id="8d896-132">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-132">Int64</span></span>   | <span data-ttu-id="8d896-133">A contagem de membros do grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-133">The group member count.</span></span>                  |
| <span data-ttu-id="8d896-134">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="8d896-134">externalMemberCount</span></span>               | <span data-ttu-id="8d896-135">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-135">Int64</span></span>   | <span data-ttu-id="8d896-136">A contagem de membros externos do grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-136">The group external member count.</span></span>         |
| <span data-ttu-id="8d896-137">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="8d896-137">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="8d896-138">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-138">Int64</span></span>   | <span data-ttu-id="8d896-139">O número de emails que a caixa de correio do grupo recebeu.</span><span class="sxs-lookup"><span data-stu-id="8d896-139">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="8d896-140">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="8d896-140">sharePointActiveFileCount</span></span>         | <span data-ttu-id="8d896-141">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-141">Int64</span></span>   | <span data-ttu-id="8d896-142">O número de arquivos ativos no site do Grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d896-142">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="8d896-143">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="8d896-143">yammerPostedMessageCount</span></span>          | <span data-ttu-id="8d896-144">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-144">Int64</span></span>   | <span data-ttu-id="8d896-145">O número de mensagens postadas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d896-145">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="8d896-146">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="8d896-146">yammerReadMessageCount</span></span>            | <span data-ttu-id="8d896-147">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-147">Int64</span></span>   | <span data-ttu-id="8d896-148">O número de mensagens lidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d896-148">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="8d896-149">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="8d896-149">yammerLikedMessageCount</span></span>           | <span data-ttu-id="8d896-150">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-150">Int64</span></span>   | <span data-ttu-id="8d896-151">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="8d896-151">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="8d896-152">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="8d896-152">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="8d896-153">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-153">Int64</span></span>   | <span data-ttu-id="8d896-154">O número de itens na caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-154">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="8d896-155">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="8d896-155">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="8d896-156">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-156">Int64</span></span>   | <span data-ttu-id="8d896-157">O armazenamento usado da caixa de correio do grupo.</span><span class="sxs-lookup"><span data-stu-id="8d896-157">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="8d896-158">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="8d896-158">sharePointTotalFileCount</span></span>          | <span data-ttu-id="8d896-159">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-159">Int64</span></span>   | <span data-ttu-id="8d896-160">O número total de arquivos no site do Grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d896-160">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="8d896-161">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="8d896-161">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="8d896-162">Int64</span><span class="sxs-lookup"><span data-stu-id="8d896-162">Int64</span></span>   | <span data-ttu-id="8d896-163">O armazenamento usado pelo site do Grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="8d896-163">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="8d896-164">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="8d896-164">reportPeriod</span></span>                      | <span data-ttu-id="8d896-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8d896-165">String</span></span>  | <span data-ttu-id="8d896-166">O número de dias que o relatório abrange.</span><span class="sxs-lookup"><span data-stu-id="8d896-166">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="8d896-167">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8d896-167">JSON representation</span></span>

<span data-ttu-id="8d896-168">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8d896-168">The following is a JSON representation of the resource.</span></span>

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


