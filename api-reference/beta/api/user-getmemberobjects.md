---
title: 'user: getMemberObjects'
description: Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.
localization_priority: Normal
ms.openlocfilehash: 68475bd93343a8be2d104891ecbc1cc7bed06482
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825743"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="a3f8e-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="a3f8e-104">user: getMemberObjects</span></span>

> <span data-ttu-id="a3f8e-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3f8e-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a3f8e-p103">Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-p103">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3f8e-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3f8e-109">Permissions</span></span>
<span data-ttu-id="a3f8e-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a3f8e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a3f8e-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3f8e-112">Permission type</span></span>      | <span data-ttu-id="a3f8e-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3f8e-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3f8e-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3f8e-114">Delegated (work or school account)</span></span> | <span data-ttu-id="a3f8e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a3f8e-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a3f8e-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3f8e-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3f8e-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-117">Not supported.</span></span>    |
|<span data-ttu-id="a3f8e-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3f8e-118">Application</span></span> | <span data-ttu-id="a3f8e-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3f8e-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3f8e-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3f8e-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="a3f8e-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a3f8e-121">Request headers</span></span>
| <span data-ttu-id="a3f8e-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a3f8e-122">Header</span></span>       | <span data-ttu-id="a3f8e-123">Valor</span><span class="sxs-lookup"><span data-stu-id="a3f8e-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3f8e-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a3f8e-124">Authorization</span></span>  | <span data-ttu-id="a3f8e-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3f8e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3f8e-127">Content-Type</span></span>  | <span data-ttu-id="a3f8e-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a3f8e-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3f8e-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3f8e-129">Request body</span></span>
<span data-ttu-id="a3f8e-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a3f8e-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a3f8e-131">Parameter</span></span>    | <span data-ttu-id="a3f8e-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3f8e-132">Type</span></span>   |<span data-ttu-id="a3f8e-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3f8e-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3f8e-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a3f8e-134">securityEnabledOnly</span></span>|<span data-ttu-id="a3f8e-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="a3f8e-135">Boolean</span></span>|<span data-ttu-id="a3f8e-p106">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-p106">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="a3f8e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3f8e-138">Response</span></span>

<span data-ttu-id="a3f8e-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos e das funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-139">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="a3f8e-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3f8e-140">Example</span></span>
<span data-ttu-id="a3f8e-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a3f8e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a3f8e-142">Request</span></span>
<span data-ttu-id="a3f8e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="a3f8e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3f8e-144">Response</span></span>
<span data-ttu-id="a3f8e-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a3f8e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
