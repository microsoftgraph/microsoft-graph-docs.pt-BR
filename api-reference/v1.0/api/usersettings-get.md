---
title: Obter configurações
description: Leia o usuário e o objeto de configurações da organização.
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a71d34dc623a54936bfdaf4db73813948cc8d3a
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844969"
---
# <a name="get-settings"></a><span data-ttu-id="9d57f-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="9d57f-103">Get settings</span></span>

<span data-ttu-id="9d57f-104">Leia o objeto [userSettings](../resources/usersettings.md) do usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="9d57f-104">Read the user and organization settings object.</span></span>
<span data-ttu-id="9d57f-105">Para saber como atualizar as propriedades do objeto [userSettings](../resources/usersettings.md), confira [atualizar as configurações de usuário](usersettings-update.md).</span><span class="sxs-lookup"><span data-stu-id="9d57f-105">To learn how to update the properties of the [settings](../resources/usersettings.md) object, see [update user settings](usersettings-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9d57f-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9d57f-106">Permissions</span></span>

<span data-ttu-id="9d57f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d57f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d57f-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9d57f-109">Permission type</span></span>      | <span data-ttu-id="9d57f-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9d57f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d57f-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9d57f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9d57f-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d57f-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="9d57f-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9d57f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d57f-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9d57f-114">Not supported.</span></span>    |
|<span data-ttu-id="9d57f-115">Application</span><span class="sxs-lookup"><span data-stu-id="9d57f-115">Application</span></span> | <span data-ttu-id="9d57f-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d57f-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d57f-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9d57f-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="9d57f-118">Solicitação com uma "id de usuário" ou "userPrincipalName" ficará acessível somente para o usuário ou um usuário com permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="9d57f-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="9d57f-119">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9d57f-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="9d57f-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9d57f-120">Request body</span></span>

<span data-ttu-id="9d57f-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9d57f-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9d57f-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d57f-122">Response</span></span>

<span data-ttu-id="9d57f-123">Se bem-sucedido, esse método retornará um código de resposta `200 OK` e um objeto [userSettings](../resources/usersettings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9d57f-123">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/usersettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d57f-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9d57f-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9d57f-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9d57f-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="9d57f-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="9d57f-126">Response</span></span>

<span data-ttu-id="9d57f-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9d57f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

