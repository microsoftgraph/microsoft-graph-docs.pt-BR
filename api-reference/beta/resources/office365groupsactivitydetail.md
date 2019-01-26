---
title: tipo de recurso de office365GroupsActivityDetail
description: Veja a seguir uma representação JSON do recurso.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1b467f73ed2a4a5e48cb1243c5b1326591bcd707
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575115"
---
# <a name="office365groupsactivitydetail-resource-type"></a><span data-ttu-id="954cf-103">tipo de recurso de office365GroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="954cf-103">office365GroupsActivityDetail resource type</span></span>

## <a name="properties"></a><span data-ttu-id="954cf-104">Propriedades</span><span class="sxs-lookup"><span data-stu-id="954cf-104">Properties</span></span>

| <span data-ttu-id="954cf-105">Propriedade</span><span class="sxs-lookup"><span data-stu-id="954cf-105">Property</span></span>                          | <span data-ttu-id="954cf-106">Tipo</span><span class="sxs-lookup"><span data-stu-id="954cf-106">Type</span></span>    | <span data-ttu-id="954cf-107">Descrição</span><span class="sxs-lookup"><span data-stu-id="954cf-107">Description</span></span>                              |
| :-------------------------------- | :------ | ---------------------------------------- |
| <span data-ttu-id="954cf-108">reportRefreshDate</span><span class="sxs-lookup"><span data-stu-id="954cf-108">reportRefreshDate</span></span>                 | <span data-ttu-id="954cf-109">Data</span><span class="sxs-lookup"><span data-stu-id="954cf-109">Date</span></span>    | <span data-ttu-id="954cf-110">A última data do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="954cf-110">The latest date of the content.</span></span>          |
| <span data-ttu-id="954cf-111">groupDisplayName</span><span class="sxs-lookup"><span data-stu-id="954cf-111">groupDisplayName</span></span>                  | <span data-ttu-id="954cf-112">String</span><span class="sxs-lookup"><span data-stu-id="954cf-112">String</span></span>  | <span data-ttu-id="954cf-113">O nome de exibição do grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-113">The display name of the group.</span></span>           |
| <span data-ttu-id="954cf-114">isDeleted</span><span class="sxs-lookup"><span data-stu-id="954cf-114">isDeleted</span></span>                         | <span data-ttu-id="954cf-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="954cf-115">Boolean</span></span> | <span data-ttu-id="954cf-116">Se esse usuário tiver sido excluído ou suave excluído.</span><span class="sxs-lookup"><span data-stu-id="954cf-116">Whether this user has been deleted or soft deleted.</span></span> |
| <span data-ttu-id="954cf-117">ownerPrincipalName</span><span class="sxs-lookup"><span data-stu-id="954cf-117">ownerPrincipalName</span></span>                | <span data-ttu-id="954cf-118">String</span><span class="sxs-lookup"><span data-stu-id="954cf-118">String</span></span>  | <span data-ttu-id="954cf-119">O nome de entidade do proprietário do grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-119">The group owner principal name.</span></span>          |
| <span data-ttu-id="954cf-120">lastActivityDate</span><span class="sxs-lookup"><span data-stu-id="954cf-120">lastActivityDate</span></span>                  | <span data-ttu-id="954cf-121">Data</span><span class="sxs-lookup"><span data-stu-id="954cf-121">Date</span></span>    | <span data-ttu-id="954cf-122">A data da última atividade para os seguintes cenários: email da caixa de correio recebida; de grupo usuário exibido, editado, compartilhados ou sincronizados arquivos na biblioteca de documentos do SharePoint; usuário exibir páginas do SharePoint; usuário postados, ler ou curtidas mensagens no Yammer grupos.</span><span class="sxs-lookup"><span data-stu-id="954cf-122">The last activity date for the following scenarios:  group mailbox received email; user viewed, edited, shared, or synced files in SharePoint document library; user viewed SharePoint pages; user posted, read, or liked messages in Yammer groups.</span></span> |
| <span data-ttu-id="954cf-123">groupType</span><span class="sxs-lookup"><span data-stu-id="954cf-123">groupType</span></span>                         | <span data-ttu-id="954cf-124">String</span><span class="sxs-lookup"><span data-stu-id="954cf-124">String</span></span>  | <span data-ttu-id="954cf-125">O tipo de grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-125">The group type.</span></span> <span data-ttu-id="954cf-126">Os valores possíveis são: **pública** ou **privada**.</span><span class="sxs-lookup"><span data-stu-id="954cf-126">Possible values are: **Public** or **Private**.</span></span> |
| <span data-ttu-id="954cf-127">memberCount</span><span class="sxs-lookup"><span data-stu-id="954cf-127">memberCount</span></span>                       | <span data-ttu-id="954cf-128">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-128">Int64</span></span>   | <span data-ttu-id="954cf-129">A contagem de membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-129">The group member count.</span></span>                  |
| <span data-ttu-id="954cf-130">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="954cf-130">externalMemberCount</span></span>               | <span data-ttu-id="954cf-131">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-131">Int64</span></span>   | <span data-ttu-id="954cf-132">A contagem de externo membro do grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-132">The group external member count.</span></span>         |
| <span data-ttu-id="954cf-133">exchangeReceivedEmailCount</span><span class="sxs-lookup"><span data-stu-id="954cf-133">exchangeReceivedEmailCount</span></span>        | <span data-ttu-id="954cf-134">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-134">Int64</span></span>   | <span data-ttu-id="954cf-135">O número de email que recebeu a caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-135">The number of email that the group mailbox received.</span></span> |
| <span data-ttu-id="954cf-136">sharePointActiveFileCount</span><span class="sxs-lookup"><span data-stu-id="954cf-136">sharePointActiveFileCount</span></span>         | <span data-ttu-id="954cf-137">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-137">Int64</span></span>   | <span data-ttu-id="954cf-138">O número de arquivos ativos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="954cf-138">The number of active files in SharePoint Group site.</span></span> |
| <span data-ttu-id="954cf-139">yammerPostedMessageCount</span><span class="sxs-lookup"><span data-stu-id="954cf-139">yammerPostedMessageCount</span></span>          | <span data-ttu-id="954cf-140">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-140">Int64</span></span>   | <span data-ttu-id="954cf-141">O número de mensagens postadas em grupos de Yammer.</span><span class="sxs-lookup"><span data-stu-id="954cf-141">The number of messages posted to Yammer groups.</span></span> |
| <span data-ttu-id="954cf-142">yammerReadMessageCount</span><span class="sxs-lookup"><span data-stu-id="954cf-142">yammerReadMessageCount</span></span>            | <span data-ttu-id="954cf-143">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-143">Int64</span></span>   | <span data-ttu-id="954cf-144">O número de mensagens lidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="954cf-144">The number of messages read in Yammer groups.</span></span> |
| <span data-ttu-id="954cf-145">yammerLikedMessageCount</span><span class="sxs-lookup"><span data-stu-id="954cf-145">yammerLikedMessageCount</span></span>           | <span data-ttu-id="954cf-146">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-146">Int64</span></span>   | <span data-ttu-id="954cf-147">O número de mensagens curtidas em grupos do Yammer.</span><span class="sxs-lookup"><span data-stu-id="954cf-147">The number of messages liked in Yammer groups.</span></span> |
| <span data-ttu-id="954cf-148">exchangeMailboxTotalItemCount</span><span class="sxs-lookup"><span data-stu-id="954cf-148">exchangeMailboxTotalItemCount</span></span>     | <span data-ttu-id="954cf-149">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-149">Int64</span></span>   | <span data-ttu-id="954cf-150">O número de itens na caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-150">The number of items in the group mailbox.</span></span> |
| <span data-ttu-id="954cf-151">exchangeMailboxStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="954cf-151">exchangeMailboxStorageUsedInBytes</span></span> | <span data-ttu-id="954cf-152">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-152">Int64</span></span>   | <span data-ttu-id="954cf-153">O armazenamento utilizado da caixa de correio de grupo.</span><span class="sxs-lookup"><span data-stu-id="954cf-153">The storage used of the group mailbox.</span></span>   |
| <span data-ttu-id="954cf-154">sharePointTotalFileCount</span><span class="sxs-lookup"><span data-stu-id="954cf-154">sharePointTotalFileCount</span></span>          | <span data-ttu-id="954cf-155">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-155">Int64</span></span>   | <span data-ttu-id="954cf-156">O número total de arquivos no site de grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="954cf-156">The total number of files in SharePoint Group site.</span></span> |
| <span data-ttu-id="954cf-157">sharePointSiteStorageUsedInBytes</span><span class="sxs-lookup"><span data-stu-id="954cf-157">sharePointSiteStorageUsedInBytes</span></span>  | <span data-ttu-id="954cf-158">Int64</span><span class="sxs-lookup"><span data-stu-id="954cf-158">Int64</span></span>   | <span data-ttu-id="954cf-159">O armazenamento usado pelo site do grupo do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="954cf-159">The storage used by SharePoint Group site.</span></span> |
| <span data-ttu-id="954cf-160">reportPeriod</span><span class="sxs-lookup"><span data-stu-id="954cf-160">reportPeriod</span></span>                      | <span data-ttu-id="954cf-161">String</span><span class="sxs-lookup"><span data-stu-id="954cf-161">String</span></span>  | <span data-ttu-id="954cf-162">O número de dias que abrange o relatório.</span><span class="sxs-lookup"><span data-stu-id="954cf-162">The number of days the report covers.</span></span>    |

## <a name="json-representation"></a><span data-ttu-id="954cf-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="954cf-163">JSON representation</span></span>

<span data-ttu-id="954cf-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="954cf-164">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail"
} -->

```json
{
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
