---
title: Obter configurações
description: Leia o objeto de configurações de organização e usuário.
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dcd9079956b4db8b349ba6b81bd85d8472630643
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334903"
---
# <a name="get-settings"></a><span data-ttu-id="eb72c-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="eb72c-103">Get settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb72c-104">Leia o objeto de [configurações](../resources/user-settings.md) de organização e usuário.</span><span class="sxs-lookup"><span data-stu-id="eb72c-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="eb72c-105">Para saber como atualizar as propriedades do objeto de [configurações](../resources/user-settings.md) , consulte [Update User Settings](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="eb72c-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb72c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="eb72c-106">Permissions</span></span>

<span data-ttu-id="eb72c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb72c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eb72c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="eb72c-109">Permission type</span></span>      | <span data-ttu-id="eb72c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="eb72c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb72c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="eb72c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb72c-112">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eb72c-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="eb72c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="eb72c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb72c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="eb72c-114">Not supported.</span></span>    |
|<span data-ttu-id="eb72c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="eb72c-115">Application</span></span> | <span data-ttu-id="eb72c-116">User. Read. All, User. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="eb72c-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb72c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="eb72c-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="eb72c-118">A solicitação com uma "ID de usuário" ou "userPrincipalName" só pode ser acessada pelo usuário ou por um usuário com as permissões User. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="eb72c-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="eb72c-119">Para saber mais, confira [permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="eb72c-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="eb72c-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="eb72c-120">Request body</span></span>

<span data-ttu-id="eb72c-121">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="eb72c-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eb72c-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb72c-122">Response</span></span>

<span data-ttu-id="eb72c-123">Se bem-sucedido, este método retorna um `200 OK` código de resposta e um objeto de [configurações do usuário](../resources/user-settings.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="eb72c-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb72c-124">Exemplo</span><span class="sxs-lookup"><span data-stu-id="eb72c-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="eb72c-125">Solicitação</span><span class="sxs-lookup"><span data-stu-id="eb72c-125">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="eb72c-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="eb72c-126">Response</span></span>

<span data-ttu-id="eb72c-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="eb72c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
