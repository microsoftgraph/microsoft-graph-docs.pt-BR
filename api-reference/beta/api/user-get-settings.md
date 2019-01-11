---
title: Obter configurações
description: Leia o objeto de configurações de usuário e da organização.
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: 30217d43ac453c9e3502b00ece22ac01edf0abfb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852399"
---
# <a name="get-settings"></a><span data-ttu-id="34ec4-103">Obter configurações</span><span class="sxs-lookup"><span data-stu-id="34ec4-103">Get settings</span></span>

> <span data-ttu-id="34ec4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34ec4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34ec4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34ec4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34ec4-106">Leia o objeto de [configurações](../resources/user-settings.md) de usuário e da organização.</span><span class="sxs-lookup"><span data-stu-id="34ec4-106">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="34ec4-107">Para saber como atualizar as propriedades do objeto de [configurações](../resources/user-settings.md) , consulte [Atualizar configurações de usuário](user-update-settings.md).</span><span class="sxs-lookup"><span data-stu-id="34ec4-107">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="34ec4-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="34ec4-108">Permissions</span></span>

<span data-ttu-id="34ec4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ec4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ec4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34ec4-111">Permission type</span></span>      | <span data-ttu-id="34ec4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="34ec4-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="34ec4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34ec4-113">Delegated (work or school account)</span></span> | <span data-ttu-id="34ec4-114">User.Read.All, User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ec4-114">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="34ec4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34ec4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="34ec4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ec4-116">Not supported.</span></span>    |
|<span data-ttu-id="34ec4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34ec4-117">Application</span></span> | <span data-ttu-id="34ec4-118">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ec4-118">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="34ec4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34ec4-119">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="34ec4-120">Solicitar com uma id de usuário' ' ou 'userPrincipalName' só está acessível pelo usuário ou por um usuário com as permissões User.ReadWrite.All.</span><span class="sxs-lookup"><span data-stu-id="34ec4-120">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="34ec4-121">Para saber mais, consulte [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ec4-121">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="34ec4-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34ec4-122">Request body</span></span>

<span data-ttu-id="34ec4-123">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="34ec4-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="34ec4-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ec4-124">Response</span></span>

<span data-ttu-id="34ec4-125">Se tiver êxito, este método retornará um `200 OK` objeto de [configurações de usuário](../resources/user-settings.md) e o código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34ec4-125">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34ec4-126">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34ec4-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="34ec4-127">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34ec4-127">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="34ec4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ec4-128">Response</span></span>

<span data-ttu-id="34ec4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34ec4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
