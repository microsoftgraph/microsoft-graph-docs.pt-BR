---
title: 'cloudPcUserSetting: assign'
description: Atribua uma configuração de usuário de computador na nuvem a grupos de usuários.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 5279a630f3ba9eeb684a98552e8f0184ab441098
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207102"
---
# <a name="cloudpcusersetting-assign"></a><span data-ttu-id="1cc6e-103">cloudPcUserSetting: assign</span><span class="sxs-lookup"><span data-stu-id="1cc6e-103">cloudPcUserSetting: assign</span></span>

<span data-ttu-id="1cc6e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1cc6e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1cc6e-105">Atribua [um cloudPcUserSetting a](../resources/cloudpcusersetting.md) grupos de usuários.</span><span class="sxs-lookup"><span data-stu-id="1cc6e-105">Assign a [cloudPcUserSetting](../resources/cloudpcusersetting.md) to user groups.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="1cc6e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cc6e-106">Permissions</span></span>

<span data-ttu-id="1cc6e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cc6e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1cc6e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cc6e-109">Permission type</span></span>|<span data-ttu-id="1cc6e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cc6e-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1cc6e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cc6e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1cc6e-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc6e-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="1cc6e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cc6e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1cc6e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cc6e-114">Not supported.</span></span>|
|<span data-ttu-id="1cc6e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cc6e-115">Application</span></span>|<span data-ttu-id="1cc6e-116">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1cc6e-116">CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1cc6e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc6e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/userSettings/{id}/assign
```

## <a name="request-headers"></a><span data-ttu-id="1cc6e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc6e-118">Request headers</span></span>

|<span data-ttu-id="1cc6e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1cc6e-119">Name</span></span>|<span data-ttu-id="1cc6e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc6e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1cc6e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1cc6e-121">Authorization</span></span>|<span data-ttu-id="1cc6e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cc6e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1cc6e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1cc6e-124">Content-Type</span></span>|<span data-ttu-id="1cc6e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1cc6e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1cc6e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc6e-127">Request body</span></span>

<span data-ttu-id="1cc6e-128">No corpo da solicitação, fornece uma representação JSON do [objeto cloudPcUserSettingAssignment.](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1cc6e-128">In the request body, supply a JSON representation of the [cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) object.</span></span>

|<span data-ttu-id="1cc6e-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="1cc6e-129">Parameter</span></span>|<span data-ttu-id="1cc6e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cc6e-130">Type</span></span>|<span data-ttu-id="1cc6e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cc6e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cc6e-132">assignments</span><span class="sxs-lookup"><span data-stu-id="1cc6e-132">assignments</span></span>|<span data-ttu-id="1cc6e-133">[coleção cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md)</span><span class="sxs-lookup"><span data-stu-id="1cc6e-133">[cloudPcUserSettingAssignment](../resources/cloudpcusersettingassignment.md) collection</span></span> | <span data-ttu-id="1cc6e-134">A coleção de recursos de configuração do usuário do computador na nuvem a serem atribuídos ao grupo de destino correspondente.</span><span class="sxs-lookup"><span data-stu-id="1cc6e-134">The collection of cloud PC user setting resources each to be assigned to the corresponding target group.</span></span> <span data-ttu-id="1cc6e-135">Atualmente, Microsoft 365 grupos de segurança e grupos de segurança no Azure AD são suportados.</span><span class="sxs-lookup"><span data-stu-id="1cc6e-135">Only Microsoft 365 groups and security groups in Azure AD are currently supported.</span></span> |

## <a name="response"></a><span data-ttu-id="1cc6e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc6e-136">Response</span></span>

<span data-ttu-id="1cc6e-137">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1cc6e-137">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="1cc6e-138">Exemplos</span><span class="sxs-lookup"><span data-stu-id="1cc6e-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1cc6e-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1cc6e-139">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1cc6e-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="1cc6e-140">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1cc6e-141">C#</span><span class="sxs-lookup"><span data-stu-id="1cc6e-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/cloudpcusersetting-assign-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1cc6e-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1cc6e-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/cloudpcusersetting-assign-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1cc6e-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1cc6e-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/cloudpcusersetting-assign-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1cc6e-144">Java</span><span class="sxs-lookup"><span data-stu-id="1cc6e-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/cloudpcusersetting-assign-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1cc6e-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cc6e-145">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
