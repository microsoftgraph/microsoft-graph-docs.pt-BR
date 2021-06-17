---
title: Obter cloudPcUserSetting
description: Leia as propriedades e as relações de um objeto cloudPcUserSetting.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b54797490580a4f1bda43252aed726292884b6a0
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52993628"
---
# <a name="get-cloudpcusersetting"></a><span data-ttu-id="8b7d4-103">Obter cloudPcUserSetting</span><span class="sxs-lookup"><span data-stu-id="8b7d4-103">Get cloudPcUserSetting</span></span>

<span data-ttu-id="8b7d4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b7d4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8b7d4-105">Leia as propriedades e as relações de um [objeto cloudPcUserSetting.](../resources/cloudpcusersetting.md)</span><span class="sxs-lookup"><span data-stu-id="8b7d4-105">Read the properties and relationships of a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="8b7d4-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8b7d4-106">Permissions</span></span>

<span data-ttu-id="8b7d4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b7d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b7d4-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b7d4-109">Permission type</span></span>|<span data-ttu-id="8b7d4-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="8b7d4-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b7d4-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b7d4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8b7d4-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b7d4-112">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="8b7d4-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b7d4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b7d4-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b7d4-114">Not supported.</span></span>|
|<span data-ttu-id="8b7d4-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b7d4-115">Application</span></span>|<span data-ttu-id="8b7d4-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b7d4-116">CloudPC.Read.All, CloudPC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b7d4-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b7d4-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /deviceManagement/virtualEndpoint/userSettings/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8b7d4-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="8b7d4-118">Optional query parameters</span></span>

<span data-ttu-id="8b7d4-119">Este método oferece `$select` suporte e `$expand` parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="8b7d4-119">This method supports `$select` and `$expand` OData query parameters to help customize the response.</span></span> <span data-ttu-id="8b7d4-120">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="8b7d4-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8b7d4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b7d4-121">Request headers</span></span>

| <span data-ttu-id="8b7d4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="8b7d4-122">Name</span></span>          | <span data-ttu-id="8b7d4-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b7d4-123">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="8b7d4-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b7d4-124">Authorization</span></span> | <span data-ttu-id="8b7d4-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b7d4-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8b7d4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b7d4-127">Request body</span></span>

<span data-ttu-id="8b7d4-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="8b7d4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b7d4-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b7d4-129">Response</span></span>

<span data-ttu-id="8b7d4-130">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto cloudPcUserSetting](../resources/cloudpcusersetting.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b7d4-130">If successful, this method returns a `200 OK` response code and a [cloudPcUserSetting](../resources/cloudpcusersetting.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8b7d4-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="8b7d4-131">Examples</span></span>

### <a name="example-1-get-the-properties-of-the-specified-user-setting"></a><span data-ttu-id="8b7d4-132">Exemplo 1: Obter as propriedades da configuração de usuário especificada</span><span class="sxs-lookup"><span data-stu-id="8b7d4-132">Example 1: Get the properties of the specified user setting</span></span>

#### <a name="request"></a><span data-ttu-id="8b7d4-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b7d4-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/userSettings/556092f8-92f8-5560-f892-6055f8926055
```


#### <a name="response"></a><span data-ttu-id="8b7d4-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b7d4-134">Response</span></span>
><span data-ttu-id="8b7d4-135">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b7d4-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-properties-of-the-specified-user-setting-and-expand-on-the-assignments"></a><span data-ttu-id="8b7d4-136">Exemplo 2: Obter as propriedades da configuração de usuário especificada e expandir nas atribuições</span><span class="sxs-lookup"><span data-stu-id="8b7d4-136">Example 2: Get the properties of the specified user setting and expand on the assignments</span></span>

#### <a name="request"></a><span data-ttu-id="8b7d4-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b7d4-137">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_cloudpcusersetting_2"
}
-->

``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/usersettings/b0c2d35f-3385-46c8-a6f5-6c3dfad7ffff?$expand=assignments
```


#### <a name="response"></a><span data-ttu-id="8b7d4-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b7d4-138">Response</span></span>

<span data-ttu-id="8b7d4-139">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="8b7d4-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
