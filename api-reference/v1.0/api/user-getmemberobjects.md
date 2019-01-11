---
title: 'user: getMemberObjects'
description: Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.
localization_priority: Priority
ms.openlocfilehash: 2d2c28ab41e7f9798ff1f77e1750e6303a52de34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811379"
---
# <a name="user-getmemberobjects"></a><span data-ttu-id="edbfe-104">user: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="edbfe-104">user: getMemberObjects</span></span>
<span data-ttu-id="edbfe-p102">Retorna todos os grupos e funções de diretório e unidades administrativas dos quais o usuário é membro. A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="edbfe-p102">Return all of the groups, directory roles and administrative units that the user is a member of. The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="edbfe-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="edbfe-107">Permissions</span></span>
<span data-ttu-id="edbfe-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="edbfe-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="edbfe-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="edbfe-110">Permission type</span></span>      | <span data-ttu-id="edbfe-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="edbfe-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="edbfe-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="edbfe-112">Delegated (work or school account)</span></span> | <span data-ttu-id="edbfe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="edbfe-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="edbfe-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="edbfe-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="edbfe-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="edbfe-115">Not supported.</span></span>    |
|<span data-ttu-id="edbfe-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="edbfe-116">Application</span></span> | <span data-ttu-id="edbfe-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="edbfe-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="edbfe-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="edbfe-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id | userPrincipalName}/getMemberObjects
```
## <a name="request-headers"></a><span data-ttu-id="edbfe-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="edbfe-119">Request headers</span></span>
| <span data-ttu-id="edbfe-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="edbfe-120">Header</span></span>       | <span data-ttu-id="edbfe-121">Valor</span><span class="sxs-lookup"><span data-stu-id="edbfe-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="edbfe-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="edbfe-122">Authorization</span></span>  | <span data-ttu-id="edbfe-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="edbfe-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="edbfe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="edbfe-125">Content-Type</span></span>  | <span data-ttu-id="edbfe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="edbfe-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="edbfe-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="edbfe-127">Request body</span></span>
<span data-ttu-id="edbfe-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edbfe-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="edbfe-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="edbfe-129">Parameter</span></span>    | <span data-ttu-id="edbfe-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="edbfe-130">Type</span></span>   |<span data-ttu-id="edbfe-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="edbfe-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="edbfe-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="edbfe-132">securityEnabledOnly</span></span>|<span data-ttu-id="edbfe-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="edbfe-133">Boolean</span></span>|<span data-ttu-id="edbfe-p105">**true** para especificar que somente grupos de segurança dos quais o usuário é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais o usuário é membro devem ser retornados. Observação: Definir esse parâmetro como **true** é suportado apenas ao chamar este método em um usuário.</span><span class="sxs-lookup"><span data-stu-id="edbfe-p105">**true** to specify that only security groups that the user is a member of should be returned; **false** to specify that all groups and directory roles that the user is a member of should be returned. Note: Setting this parameter to **true** is only supported when calling this method on a user.</span></span>|

## <a name="response"></a><span data-ttu-id="edbfe-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="edbfe-136">Response</span></span>

<span data-ttu-id="edbfe-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e a coleção de cadeias de caracteres no corpo da resposta que contém as IDs dos grupos e das funções de diretório dos quais o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="edbfe-137">If successful, this method returns `200 OK` response code and String collection in the response body that contains the IDs of the groups and directory roles that the user is a member of.</span></span>

## <a name="example"></a><span data-ttu-id="edbfe-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="edbfe-138">Example</span></span>
<span data-ttu-id="edbfe-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="edbfe-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="edbfe-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="edbfe-140">Request</span></span>
<span data-ttu-id="edbfe-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="edbfe-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "user_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="edbfe-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="edbfe-142">Response</span></span>
<span data-ttu-id="edbfe-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="edbfe-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
