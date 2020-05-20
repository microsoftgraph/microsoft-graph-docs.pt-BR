---
title: 'servicePrincipalName: getMemberGroups'
description: Obtenha a lista de grupos dos quais essa entidade de serviço é membro.  A verificação é transitiva.
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 5859d7834a54426dc29930b67bf7ed44ee43a431
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290367"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="58531-104">servicePrincipalName: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="58531-104">servicePrincipal: getMemberGroups</span></span>

<span data-ttu-id="58531-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58531-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="58531-106">Obtenha a lista de grupos dos quais esse [servicePrincipalName](../resources/serviceprincipal.md) é um membro.</span><span class="sxs-lookup"><span data-stu-id="58531-106">Get the list of groups that this [servicePrincipal](../resources/serviceprincipal.md) is a member of.</span></span>  <span data-ttu-id="58531-107">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="58531-107">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="58531-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="58531-108">Permissions</span></span>
<span data-ttu-id="58531-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="58531-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="58531-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58531-111">Permission type</span></span>      | <span data-ttu-id="58531-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="58531-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="58531-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58531-113">Delegated (work or school account)</span></span> | <span data-ttu-id="58531-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="58531-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="58531-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58531-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="58531-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58531-116">Not supported.</span></span>    |
|<span data-ttu-id="58531-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58531-117">Application</span></span> | <span data-ttu-id="58531-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58531-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="58531-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58531-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="58531-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58531-120">Request headers</span></span>
| <span data-ttu-id="58531-121">Nome</span><span class="sxs-lookup"><span data-stu-id="58531-121">Name</span></span>       | <span data-ttu-id="58531-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="58531-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="58531-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="58531-123">Authorization</span></span> | <span data-ttu-id="58531-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58531-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="58531-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="58531-126">Content-type</span></span> | <span data-ttu-id="58531-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58531-p105">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="58531-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58531-129">Request body</span></span>
<span data-ttu-id="58531-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58531-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="58531-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="58531-131">Parameter</span></span>    | <span data-ttu-id="58531-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="58531-132">Type</span></span>   |<span data-ttu-id="58531-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="58531-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58531-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="58531-134">securityEnabledOnly</span></span>|<span data-ttu-id="58531-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="58531-135">Boolean</span></span>|<span data-ttu-id="58531-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="58531-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="58531-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="58531-138">Response</span></span>

<span data-ttu-id="58531-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto da coleção String no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58531-139">If successful, this method returns a `200 OK` response code and a String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58531-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58531-140">Example</span></span>
<span data-ttu-id="58531-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="58531-141">Here is an example of how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="58531-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58531-142">Request</span></span>
<span data-ttu-id="58531-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58531-143">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

### <a name="response"></a><span data-ttu-id="58531-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="58531-144">Response</span></span>
<span data-ttu-id="58531-145">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58531-145">Here is an example of the response.</span></span> 
><span data-ttu-id="58531-p107">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58531-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
