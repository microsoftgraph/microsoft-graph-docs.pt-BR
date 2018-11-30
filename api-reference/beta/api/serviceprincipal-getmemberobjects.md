---
title: 'servicePrincipal: getMemberObjects'
description: Obter a lista de grupos e funções de diretório que esse serviço principal é um membro de.  Essa verificação é transitiva.
ms.openlocfilehash: 82fd1791b32c54a4670977e7ca5a66bdd92c1c14
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037906"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="fc4c4-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="fc4c4-104">servicePrincipal: getMemberObjects</span></span>

> <span data-ttu-id="fc4c4-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc4c4-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fc4c4-107">Obter a lista de grupos e funções de diretório que esse serviço principal é um membro de.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-107">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="fc4c4-108">Essa verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-108">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc4c4-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="fc4c4-109">Permissions</span></span>
<span data-ttu-id="fc4c4-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc4c4-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc4c4-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fc4c4-112">Permission type</span></span>      | <span data-ttu-id="fc4c4-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fc4c4-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc4c4-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fc4c4-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fc4c4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc4c4-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc4c4-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fc4c4-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc4c4-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-117">Not supported.</span></span>    |
|<span data-ttu-id="fc4c4-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fc4c4-118">Application</span></span> | <span data-ttu-id="fc4c4-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc4c4-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc4c4-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fc4c4-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="fc4c4-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fc4c4-121">Request headers</span></span>
| <span data-ttu-id="fc4c4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="fc4c4-122">Name</span></span>       | <span data-ttu-id="fc4c4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc4c4-123">Type</span></span> | <span data-ttu-id="fc4c4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc4c4-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="fc4c4-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fc4c4-125">Authorization</span></span>  | <span data-ttu-id="fc4c4-126">string</span><span class="sxs-lookup"><span data-stu-id="fc4c4-126">string</span></span>  | <span data-ttu-id="fc4c4-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc4c4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fc4c4-129">Request body</span></span>
<span data-ttu-id="fc4c4-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="fc4c4-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="fc4c4-131">Parameter</span></span>    | <span data-ttu-id="fc4c4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="fc4c4-132">Type</span></span>   |<span data-ttu-id="fc4c4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="fc4c4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fc4c4-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="fc4c4-134">securityEnabledOnly</span></span>|<span data-ttu-id="fc4c4-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="fc4c4-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="fc4c4-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc4c4-136">Response</span></span>

<span data-ttu-id="fc4c4-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc4c4-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fc4c4-138">Example</span></span>
<span data-ttu-id="fc4c4-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fc4c4-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fc4c4-140">Request</span></span>
<span data-ttu-id="fc4c4-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "serviceprincipal_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/getMemberObjects
Content-type: application/json
Content-length: 33

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="fc4c4-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fc4c4-142">Response</span></span>
<span data-ttu-id="fc4c4-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fc4c4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "servicePrincipal: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->