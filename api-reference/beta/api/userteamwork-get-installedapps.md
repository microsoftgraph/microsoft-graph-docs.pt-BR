---
title: Obter o aplicativo instalado para o usuário
description: Recupere o aplicativo instalado no escopo pessoal do usuário especificado.
author: AkJo
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 393a0663136ec167645a93cfcedd776758ed88d2
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564142"
---
# <a name="get-installed-app-for-user"></a><span data-ttu-id="73178-103">Obter o aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="73178-103">Get installed app for user</span></span>

<span data-ttu-id="73178-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73178-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73178-105">Recupere o [aplicativo](../resources/teamsappinstallation.md) instalado no escopo pessoal do [usuário](../resources/user.md)especificado.</span><span class="sxs-lookup"><span data-stu-id="73178-105">Retrieve the [app](../resources/teamsappinstallation.md) installed in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="73178-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="73178-106">Permissions</span></span>

<span data-ttu-id="73178-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="73178-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73178-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="73178-109">Permission type</span></span>      | <span data-ttu-id="73178-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="73178-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="73178-111">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="73178-111">Delegated (work or school account)</span></span> | <span data-ttu-id="73178-112">TeamsAppInstallation. ReadForUser, TeamsAppInstallation. Read, TeamsAppInstallation. ReadWriteSelfForUser, TeamsAppInstallation. ReadWriteForUser, TeamsAppInstallation. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="73178-112">TeamsAppInstallation.ReadForUser, TeamsAppInstallation.Read, TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="73178-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="73178-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73178-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="73178-114">Not supported.</span></span>    |
|<span data-ttu-id="73178-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="73178-115">Application</span></span> | <span data-ttu-id="73178-116">TeamsAppInstallation. ReadForUser. All, TeamsAppInstallation. Read. All, TeamsAppInstallation. ReadWriteSelfForUser. All, TeamsAppInstallation. ReadWriteForUser. All, TeamsAppInstallation. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="73178-116">TeamsAppInstallation.ReadForUser.All, TeamsAppInstallation.Read.All, TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="73178-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="73178-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id}/teamwork/installedApps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="73178-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="73178-118">Request headers</span></span>

| <span data-ttu-id="73178-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="73178-119">Header</span></span>       | <span data-ttu-id="73178-120">Valor</span><span class="sxs-lookup"><span data-stu-id="73178-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="73178-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="73178-121">Authorization</span></span>  | <span data-ttu-id="73178-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="73178-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="73178-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="73178-124">Request body</span></span>

<span data-ttu-id="73178-125">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="73178-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73178-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="73178-126">Response</span></span>

<span data-ttu-id="73178-127">Se tiver êxito, este método retornará um `200 OK` código de resposta e um [aplicativo](../resources/teamsappinstallation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="73178-127">If successful, this method returns a `200 OK` response code and an [app](../resources/teamsappinstallation.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="73178-128">Exemplos</span><span class="sxs-lookup"><span data-stu-id="73178-128">Examples</span></span>

### <a name="example-1-get-an-app-installed-for-the-specified-user"></a><span data-ttu-id="73178-129">Exemplo 1: obter um aplicativo instalado para o usuário especificado</span><span class="sxs-lookup"><span data-stu-id="73178-129">Example 1: Get an app installed for the specified user</span></span>

#### <a name="request"></a><span data-ttu-id="73178-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73178-130">Request</span></span>

<span data-ttu-id="73178-131">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73178-131">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_list_teamsApps"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/users/{id}/teamwork/installedApps/{id}
```

#### <a name="response"></a><span data-ttu-id="73178-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="73178-132">Response</span></span>

<span data-ttu-id="73178-133">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73178-133">The following is an example of the response.</span></span>
><span data-ttu-id="73178-p103">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73178-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```
### <a name="example-2-get-the-names-and-other-details-of-the-app-installed-for-the-user"></a><span data-ttu-id="73178-136">Exemplo 2: obter os nomes e outros detalhes do aplicativo instalado para o usuário</span><span class="sxs-lookup"><span data-stu-id="73178-136">Example 2: Get the names and other details of the app installed for the user</span></span>

#### <a name="request"></a><span data-ttu-id="73178-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="73178-137">Request</span></span>

<span data-ttu-id="73178-138">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="73178-138">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "user_list_teamsApps_details"
}-->
```http
GET https://graph.microsoft.com/beta/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=?$expand=teamsAppDefinition
```

#### <a name="response"></a><span data-ttu-id="73178-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="73178-139">Response</span></span>

<span data-ttu-id="73178-140">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="73178-140">The following is an example of the response.</span></span>

><span data-ttu-id="73178-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="73178-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_list_teamsApps_details",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation",
  "isCollection": false
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
        {
          "@odata.context": "https://graph.microsoft.com/beta/$metadata#teams('5b649834-7412-4cce-9e69-176e95a394f5')/installedApps(teamsAppDefinition())/$entity",
          "id": "NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk=",
          "teamsAppDefinition": {
                                  "id": "YTZiNjMzNjUtMzFhNC00ZjQzLTkyZWMtNzEwYjcxNTU3YWY5IyMwLjk=",
                                  "teamsAppId": "a6b63365-31a4-4f43-92ec-710b71557af9",
                                  "displayName": "Power Apps",
                                  "version": "0.9"
                                }
          }
         ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User get teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
