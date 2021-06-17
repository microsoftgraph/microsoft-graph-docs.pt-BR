---
title: 'cloudPcUserSetting: assign'
description: Atribua uma configuração de usuário de computador na nuvem a grupos de usuários.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 987ecf4ee31b2ade7baf08246542b13d14a3a6da
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993629"
---
# <a name="cloudpcusersetting-assign"></a><span data-ttu-id="f1f72-103">cloudPcUserSetting: assign</span><span class="sxs-lookup"><span data-stu-id="f1f72-103">cloudPcUserSetting: assign</span></span>

<span data-ttu-id="f1f72-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f1f72-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1f72-105">Atribua [um cloudPcUserSetting a](../resources/cloudpcusersetting.md) grupos de usuários.</span><span class="sxs-lookup"><span data-stu-id="f1f72-105">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="f1f72-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="f1f72-106">Permissions</span></span>

<span data-ttu-id="f1f72-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1f72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1f72-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1f72-109">Permission type</span></span>|<span data-ttu-id="f1f72-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f1f72-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1f72-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1f72-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f1f72-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f72-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f1f72-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1f72-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1f72-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1f72-114">Not supported.</span></span>|
|<span data-ttu-id="f1f72-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1f72-115">Application</span></span>|<span data-ttu-id="f1f72-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f72-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1f72-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1f72-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="f1f72-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f72-118">Request headers</span></span>

|<span data-ttu-id="f1f72-119">Nome</span><span class="sxs-lookup"><span data-stu-id="f1f72-119">Name</span></span>|<span data-ttu-id="f1f72-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f72-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f1f72-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1f72-121">Authorization</span></span>|<span data-ttu-id="f1f72-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1f72-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f1f72-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f1f72-124">Content-Type</span></span>|<span data-ttu-id="f1f72-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1f72-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1f72-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f72-127">Request body</span></span>

<span data-ttu-id="f1f72-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcUserSettingAssignment.](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f1f72-128">In the request body, supply a JSON representation of the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) object.</span></span>

<span data-ttu-id="f1f72-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md).</span><span class="sxs-lookup"><span data-stu-id="f1f72-129">The following table shows the properties that are required when you create the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md).</span></span>

|<span data-ttu-id="f1f72-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1f72-130">Property</span></span>|<span data-ttu-id="f1f72-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1f72-131">Type</span></span>|<span data-ttu-id="f1f72-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1f72-133">destino</span><span class="sxs-lookup"><span data-stu-id="f1f72-133">target</span></span>|[<span data-ttu-id="f1f72-134">cloudPcManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f1f72-134">cloudPcManagementAssignmentTarget</span></span>](../resources/cloudpcmanagementassignmenttarget.md)|<span data-ttu-id="f1f72-135">O destino da atribuição da política de provisionamento.</span><span class="sxs-lookup"><span data-stu-id="f1f72-135">The assignment target for the provisioning policy.</span></span> <span data-ttu-id="f1f72-136">Atualmente, o único destino com suporte é um grupo de usuários.</span><span class="sxs-lookup"><span data-stu-id="f1f72-136">Currently, the only target supported is a user group.</span></span>|

## <a name="response"></a><span data-ttu-id="f1f72-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f72-137">Response</span></span>

<span data-ttu-id="f1f72-138">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="f1f72-138">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f1f72-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f1f72-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f1f72-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f72-140">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "cloudpcusersetting_assign"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff/assign
Content-Type: application/json
Content-length: 254

{
  "assignments": [
    {
      "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
      "target":{
        "@odata.type": "microsoft.graph.cloudPcManagementGroupAssignmentTarget",
        "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26ffff"
        }
    }
  ]
}
```


### <a name="response"></a><span data-ttu-id="f1f72-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f72-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
