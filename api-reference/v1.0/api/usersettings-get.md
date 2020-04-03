---
title: Obter configurações
description: Leia o usuário e o objeto de configurações da organização.
author: krbain
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 5c13fc7b26b7d83ceda3a9c16d5a0d801f4f49c1
ms.sourcegitcommit: d6386c5d4bb8917132c3f6c4de945487939b7fb7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2020
ms.locfileid: "43109037"
---
# <a name="get-settings"></a><span data-ttu-id="c26ca-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="c26ca-103">Get settings</span></span>

<span data-ttu-id="c26ca-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c26ca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c26ca-105">Leia o objeto [userSettings](../resources/usersettings.md) do usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="c26ca-105">Read the user and organization [userSettings](../resources/usersettings.md) object.</span></span>
<span data-ttu-id="c26ca-106">Para saber como atualizar as propriedades do objeto [userSettings](../resources/usersettings.md), confira [atualizar as configurações de usuário](usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="c26ca-106">To learn how to update the properties of the [userSettings](../resources/usersettings.md) object, see [update user settings](usersettings-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c26ca-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="c26ca-107">Permissions</span></span>

<span data-ttu-id="c26ca-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c26ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c26ca-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c26ca-110">Permission type</span></span>      | <span data-ttu-id="c26ca-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c26ca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c26ca-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c26ca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c26ca-113">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26ca-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="c26ca-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c26ca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c26ca-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c26ca-115">Not supported.</span></span>    |
|<span data-ttu-id="c26ca-116">Application</span><span class="sxs-lookup"><span data-stu-id="c26ca-116">Application</span></span> | <span data-ttu-id="c26ca-117">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c26ca-117">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c26ca-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c26ca-118">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="c26ca-119">Solicitação com uma "id de usuário" ou "userPrincipalName" ficará acessível somente para o usuário ou um usuário com permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="c26ca-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="c26ca-120">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c26ca-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="c26ca-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c26ca-121">Request body</span></span>

<span data-ttu-id="c26ca-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c26ca-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c26ca-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="c26ca-123">Response</span></span>

<span data-ttu-id="c26ca-124">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [userSettings](../resources/usersettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c26ca-124">If successful, this method returns a `200 OK` response code and [userSettings](../resources/usersettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c26ca-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c26ca-125">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c26ca-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c26ca-126">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="c26ca-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="c26ca-127">Response</span></span>

<span data-ttu-id="c26ca-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c26ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

