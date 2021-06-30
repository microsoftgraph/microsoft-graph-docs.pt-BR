---
title: Obter cloudPcUserSetting
description: Leia as propriedades e as relações de um objeto cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 7b3361b2c0ed7fdf2d97890aec78ef336912aeb2
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207284"
---
# <a name="get-cloudpcusersetting"></a><span data-ttu-id="40034-103">Obter cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="40034-103">Get cloudPcUserSetting</span></span>

<span data-ttu-id="40034-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40034-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40034-105">Leia as propriedades e as relações de um [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="40034-105">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="40034-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="40034-106">Permissions</span></span>

<span data-ttu-id="40034-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40034-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40034-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40034-109">Permission type</span></span>|<span data-ttu-id="40034-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="40034-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40034-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40034-111">Delegated (work or school account)</span></span>|<span data-ttu-id="40034-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40034-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="40034-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40034-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40034-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40034-114">Not supported.</span></span>|
|<span data-ttu-id="40034-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40034-115">Application</span></span>|<span data-ttu-id="40034-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40034-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40034-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40034-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="40034-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="40034-118">Optional query parameters</span></span>

<span data-ttu-id="40034-119">Este método oferece `$select` suporte e `$expand` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="40034-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="40034-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="40034-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="40034-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40034-121">Request headers</span></span>

| <span data-ttu-id="40034-122">Nome</span><span class="sxs-lookup"><span data-stu-id="40034-122">Name</span></span>          | <span data-ttu-id="40034-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="40034-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="40034-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="40034-124">Authorization</span></span> | <span data-ttu-id="40034-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40034-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="40034-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40034-127">Request body</span></span>

<span data-ttu-id="40034-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="40034-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="40034-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="40034-129">Response</span></span>

<span data-ttu-id="40034-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcUserSetting](../resources/cloudpcusersetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40034-130">If successful, this method returns a `200 OK` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="40034-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="40034-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-user-setting"></a><span data-ttu-id="40034-132">Exemplo 1: Obter as propriedades da configuração de usuário especificada</span><span class="sxs-lookup"><span data-stu-id="40034-132">Example 1: Get the properties of the specified user setting</span></span>

#### <a name="request"></a><span data-ttu-id="40034-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40034-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40034-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="40034-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055
```
# <a name="c"></a>[<span data-ttu-id="40034-135">C#</span><span class="sxs-lookup"><span data-stu-id="40034-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcusersetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40034-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40034-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcusersetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40034-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40034-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcusersetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40034-138">Java</span><span class="sxs-lookup"><span data-stu-id="40034-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcusersetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="40034-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="40034-139">Response</span></span>
><span data-ttu-id="40034-140">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40034-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "556092f8-92f8-5560-f892-6055f8926055",
    "displayName": "String",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z"
  }
}
```

### <a name="example-2-get-the-properties-of-the-specified-user-setting-and-expand-on-the-assignments"></a><span data-ttu-id="40034-141">Exemplo 2: Obter as propriedades da configuração de usuário especificada e expandir nas atribuições</span><span class="sxs-lookup"><span data-stu-id="40034-141">Example 2: Get the properties of the specified user setting and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="40034-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40034-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="40034-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="40034-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff?$expand=assignments
```
# <a name="c"></a>[<span data-ttu-id="40034-144">C#</span><span class="sxs-lookup"><span data-stu-id="40034-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-cloudpcusersetting-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="40034-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="40034-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-cloudpcusersetting-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="40034-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="40034-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-cloudpcusersetting-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="40034-147">Java</span><span class="sxs-lookup"><span data-stu-id="40034-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-cloudpcusersetting-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="40034-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="40034-148">Response</span></span>

<span data-ttu-id="40034-149">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="40034-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcUserSetting"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPcUserSetting",
    "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff",
    "displayName": "Display Name value",
    "selfServiceEnabled": true,
    "localAdminEnabled": false,
    "lastModifiedDateTime": "2021-02-01T10:29:57Z",
    "createdDateTime": "2021-02-01T10:29:57Z",
    "assignments": [
      {
        "@odata.type": "microsoft.graph.cloudPcUserSettingAssignment",
        "id": "b0c2d35f-3385-46c8-a6f5-6c3dfad7708b_64ff06de-9c00-4a5a-98b5-7f5abe26ffff",
        "createdDateTime": "2021-02-01T10:29:57Z",
        "target": {
          "@odata.type":"microsoft.graph.cloudPCManagementGroupAssignmentTarget",
          "groupId":"64ff06de-9c00-4a5a-98b5-7f5abe26bfd9"
          }
      }
    ]
  }
}
```
