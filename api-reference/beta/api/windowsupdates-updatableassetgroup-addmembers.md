---
title: 'updatableAssetGroup: addMembers'
description: Adicione membros a um updatableAssetGroup.
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: apiPageType
ms.openlocfilehash: 99d56de596cb28f21bffdd915911fd6ca6c9417f
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53316473"
---
# <a name="updatableassetgroup-addmembers"></a><span data-ttu-id="3837b-103">updatableAssetGroup: addMembers</span><span class="sxs-lookup"><span data-stu-id="3837b-103">updatableAssetGroup: addMembers</span></span>
<span data-ttu-id="3837b-104">Namespace: microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="3837b-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3837b-105">Adicionar membros a [um updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span><span class="sxs-lookup"><span data-stu-id="3837b-105">Add members to an [updatableAssetGroup](../resources/windowsupdates-updatableassetgroup.md).</span></span>

<span data-ttu-id="3837b-106">Você pode adicionar [recursos do azureADDevice](../resources/windowsupdates-azureaddevice.md) como membros, mas pode não adicionar **recursos updatableAssetGroup** como membros.</span><span class="sxs-lookup"><span data-stu-id="3837b-106">You can add [azureADDevice](../resources/windowsupdates-azureaddevice.md) resources as members, but may not add **updatableAssetGroup** resources as members.</span></span>

<span data-ttu-id="3837b-107">Adicionar um dispositivo do Azure AD como membro de um grupo de ativos atualizável cria automaticamente um **objeto azureADDevice,** se ainda não existir.</span><span class="sxs-lookup"><span data-stu-id="3837b-107">Adding an Azure AD device as a member of an updatable asset group automatically creates an **azureADDevice** object, if it does not already exist.</span></span>

<span data-ttu-id="3837b-108">Você também pode usar o [método addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) para adicionar membros.</span><span class="sxs-lookup"><span data-stu-id="3837b-108">You can also use the method [addMembersById](windowsupdates-updatableassetgroup-addmembersbyid.md) to add members.</span></span>

## <a name="permissions"></a><span data-ttu-id="3837b-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3837b-109">Permissions</span></span>
<span data-ttu-id="3837b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3837b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3837b-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3837b-112">Permission type</span></span>|<span data-ttu-id="3837b-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3837b-113">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3837b-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3837b-114">Delegated (work or school account)</span></span>|<span data-ttu-id="3837b-115">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3837b-115">WindowsUpdates.ReadWrite.All</span></span>|
|<span data-ttu-id="3837b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3837b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3837b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3837b-117">Not supported.</span></span>|
|<span data-ttu-id="3837b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3837b-118">Application</span></span>|<span data-ttu-id="3837b-119">WindowsUpdates.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3837b-119">WindowsUpdates.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3837b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3837b-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembers
```

## <a name="request-headers"></a><span data-ttu-id="3837b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3837b-121">Request headers</span></span>
|<span data-ttu-id="3837b-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3837b-122">Name</span></span>|<span data-ttu-id="3837b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3837b-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3837b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3837b-124">Authorization</span></span>|<span data-ttu-id="3837b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3837b-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="3837b-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3837b-127">Content-Type</span></span>|<span data-ttu-id="3837b-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3837b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3837b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3837b-130">Request body</span></span>
<span data-ttu-id="3837b-131">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="3837b-131">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="3837b-132">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="3837b-132">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="3837b-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3837b-133">Parameter</span></span>|<span data-ttu-id="3837b-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="3837b-134">Type</span></span>|<span data-ttu-id="3837b-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="3837b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3837b-136">assets</span><span class="sxs-lookup"><span data-stu-id="3837b-136">assets</span></span>|<span data-ttu-id="3837b-137">[coleção microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md)</span><span class="sxs-lookup"><span data-stu-id="3837b-137">[microsoft.graph.windowsUpdates.updatableAsset](../resources/windowsupdates-updatableasset.md) collection</span></span>|<span data-ttu-id="3837b-138">Lista de **recursos updatableAsset** a adicionar como membros do **updatableAssetGroup**.</span><span class="sxs-lookup"><span data-stu-id="3837b-138">List of **updatableAsset** resources to add as members of the **updatableAssetGroup**.</span></span>|

## <a name="response"></a><span data-ttu-id="3837b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="3837b-139">Response</span></span>

<span data-ttu-id="3837b-140">Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.</span><span class="sxs-lookup"><span data-stu-id="3837b-140">If successful, this action returns a `202 Accepted` response code.</span></span> <span data-ttu-id="3837b-141">Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3837b-141">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3837b-142">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3837b-142">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3837b-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3837b-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "updatableassetgroup_addmembers"
}
-->
``` http
POST https://graph.microsoft.com/beta/admin/windows/updates/updatableAssets/{updatableAssetGroupId}/addMembers
Content-Type: application/json

{
  "assets": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdates.azureADDevice",
      "id": "String (identifier)"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="3837b-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="3837b-144">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
