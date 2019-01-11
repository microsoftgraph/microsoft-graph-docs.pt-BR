---
title: 'servicePrincipal: getMemberObjects'
description: Obter a lista de grupos e funções de diretório que esse serviço principal é um membro de.  Essa verificação é transitiva.
localization_priority: Normal
ms.openlocfilehash: 46c23e18d2484b3dff38ed8791f203e823c4cc9c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842116"
---
# <a name="serviceprincipal-getmemberobjects"></a><span data-ttu-id="f4ae7-104">servicePrincipal: getMemberObjects</span><span class="sxs-lookup"><span data-stu-id="f4ae7-104">servicePrincipal: getMemberObjects</span></span>

> <span data-ttu-id="f4ae7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4ae7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f4ae7-107">Obter a lista de grupos e funções de diretório que esse serviço principal é um membro de.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-107">Get the list of groups and directory roles that this service principal is a member of.</span></span>  <span data-ttu-id="f4ae7-108">Essa verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-108">This check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4ae7-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="f4ae7-109">Permissions</span></span>
<span data-ttu-id="f4ae7-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4ae7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4ae7-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4ae7-112">Permission type</span></span>      | <span data-ttu-id="f4ae7-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f4ae7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4ae7-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4ae7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f4ae7-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4ae7-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4ae7-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4ae7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4ae7-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-117">Not supported.</span></span>    |
|<span data-ttu-id="f4ae7-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4ae7-118">Application</span></span> | <span data-ttu-id="f4ae7-119">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4ae7-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4ae7-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4ae7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="f4ae7-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ae7-121">Request headers</span></span>
| <span data-ttu-id="f4ae7-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f4ae7-122">Name</span></span>       | <span data-ttu-id="f4ae7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ae7-123">Type</span></span> | <span data-ttu-id="f4ae7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ae7-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f4ae7-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4ae7-125">Authorization</span></span>  | <span data-ttu-id="f4ae7-126">string</span><span class="sxs-lookup"><span data-stu-id="f4ae7-126">string</span></span>  | <span data-ttu-id="f4ae7-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f4ae7-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ae7-129">Request body</span></span>
<span data-ttu-id="f4ae7-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f4ae7-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f4ae7-131">Parameter</span></span>    | <span data-ttu-id="f4ae7-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4ae7-132">Type</span></span>   |<span data-ttu-id="f4ae7-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4ae7-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4ae7-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f4ae7-134">securityEnabledOnly</span></span>|<span data-ttu-id="f4ae7-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4ae7-135">Boolean</span></span>||

## <a name="response"></a><span data-ttu-id="f4ae7-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4ae7-136">Response</span></span>

<span data-ttu-id="f4ae7-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4ae7-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4ae7-138">Example</span></span>
<span data-ttu-id="f4ae7-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f4ae7-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4ae7-140">Request</span></span>
<span data-ttu-id="f4ae7-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="f4ae7-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4ae7-142">Response</span></span>
<span data-ttu-id="f4ae7-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4ae7-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
