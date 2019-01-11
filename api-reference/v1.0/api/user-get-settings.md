---
title: Obter configurações
description: Leia o objeto de configurações de usuário e da organização.
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: ace7c43b27860832968572628838484bc8c91c84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815488"
---
# <a name="get-settings"></a><span data-ttu-id="acc2a-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="acc2a-103">Get settings</span></span>

<span data-ttu-id="acc2a-104">Leia o objeto de [configurações](../resources/user-settings.md) de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="acc2a-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="acc2a-105">Para saber como atualizar as propriedades do objeto de [configurações](../resources/user-settings.md) , consulte [Atualizar configurações de usuário](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="acc2a-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="acc2a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="acc2a-106">Permissions</span></span>

<span data-ttu-id="acc2a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acc2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acc2a-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="acc2a-109">Permission type</span></span>      | <span data-ttu-id="acc2a-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="acc2a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acc2a-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="acc2a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="acc2a-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acc2a-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="acc2a-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="acc2a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acc2a-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="acc2a-114">Not supported.</span></span>    |
|<span data-ttu-id="acc2a-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="acc2a-115">Application</span></span> | <span data-ttu-id="acc2a-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="acc2a-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="acc2a-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="acc2a-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="acc2a-118">Solicitar com uma id de usuário' ' ou 'userPrincipalName' só está acessível pelo usuário ou por um usuário com as permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="acc2a-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="acc2a-119">Para saber mais, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acc2a-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="acc2a-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="acc2a-120">Request body</span></span>

<span data-ttu-id="acc2a-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="acc2a-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acc2a-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="acc2a-122">Response</span></span>

<span data-ttu-id="acc2a-123">Se tiver êxito, este método retornará um `200 OK` objeto de [configurações de usuário](../resources/user-settings.md) e o código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="acc2a-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acc2a-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="acc2a-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="acc2a-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="acc2a-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="acc2a-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="acc2a-126">Response</span></span>

<span data-ttu-id="acc2a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="acc2a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

