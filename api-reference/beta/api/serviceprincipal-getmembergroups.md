---
title: 'servicePrincipal: getMemberGroups'
description: Obter a lista de grupos que essa entidade de serviço é um membro de.  A seleção é transitiva.
localization_priority: Normal
ms.openlocfilehash: 6d552b410da23e5675257340ddc61cb4abbcd5e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817644"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="4e119-104">servicePrincipal: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="4e119-104">servicePrincipal: getMemberGroups</span></span>

> <span data-ttu-id="4e119-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4e119-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e119-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4e119-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e119-107">Obter a lista de grupos que essa entidade de serviço é um membro de.</span><span class="sxs-lookup"><span data-stu-id="4e119-107">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="4e119-108">A seleção é transitiva.</span><span class="sxs-lookup"><span data-stu-id="4e119-108">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e119-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="4e119-109">Permissions</span></span>
<span data-ttu-id="4e119-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4e119-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e119-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4e119-112">Permission type</span></span>      | <span data-ttu-id="4e119-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4e119-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e119-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4e119-114">Delegated (work or school account)</span></span> | <span data-ttu-id="4e119-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4e119-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4e119-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4e119-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e119-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4e119-117">Not supported.</span></span>    |
|<span data-ttu-id="4e119-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4e119-118">Application</span></span> | <span data-ttu-id="4e119-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4e119-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e119-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4e119-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="4e119-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4e119-121">Request headers</span></span>
| <span data-ttu-id="4e119-122">Nome</span><span class="sxs-lookup"><span data-stu-id="4e119-122">Name</span></span>       | <span data-ttu-id="4e119-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e119-123">Type</span></span> | <span data-ttu-id="4e119-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e119-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="4e119-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="4e119-125">Authorization</span></span>  | <span data-ttu-id="4e119-126">string</span><span class="sxs-lookup"><span data-stu-id="4e119-126">string</span></span>  | <span data-ttu-id="4e119-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4e119-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e119-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4e119-129">Request body</span></span>
<span data-ttu-id="4e119-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e119-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="4e119-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="4e119-131">Parameter</span></span>    | <span data-ttu-id="4e119-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e119-132">Type</span></span>   |<span data-ttu-id="4e119-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e119-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e119-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="4e119-134">securityEnabledOnly</span></span>|<span data-ttu-id="4e119-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="4e119-135">Boolean</span></span>|<span data-ttu-id="4e119-p106">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="4e119-p106">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="4e119-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e119-138">Response</span></span>

<span data-ttu-id="4e119-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4e119-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4e119-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4e119-140">Example</span></span>
<span data-ttu-id="4e119-141">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="4e119-141">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="4e119-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4e119-142">Request</span></span>
<span data-ttu-id="4e119-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4e119-143">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberGroups
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="4e119-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="4e119-144">Response</span></span>
<span data-ttu-id="4e119-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4e119-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
