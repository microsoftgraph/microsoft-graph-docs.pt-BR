---
title: 'servicePrincipalName: getMemberGroups'
description: Obtenha a lista de grupos dos quais essa entidade de serviço é membro.  A verificação é transitiva.
localization_priority: Normal
ms.openlocfilehash: 80d81444b9e70bd27b5bc5346ffa0e42e9371837
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545465"
---
# <a name="serviceprincipal-getmembergroups"></a><span data-ttu-id="a4a6b-104">servicePrincipalName: getMemberGroups</span><span class="sxs-lookup"><span data-stu-id="a4a6b-104">servicePrincipal: getMemberGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4a6b-105">Obtenha a lista de grupos dos quais essa entidade de serviço é membro.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-105">Get the list of groups that this service principal is a member of.</span></span>  <span data-ttu-id="a4a6b-106">A verificação é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-106">The check is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="a4a6b-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a4a6b-107">Permissions</span></span>
<span data-ttu-id="a4a6b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4a6b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a4a6b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a4a6b-110">Permission type</span></span>      | <span data-ttu-id="a4a6b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a4a6b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a4a6b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a4a6b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a4a6b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a4a6b-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a4a6b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a4a6b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a4a6b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-115">Not supported.</span></span>    |
|<span data-ttu-id="a4a6b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a4a6b-116">Application</span></span> | <span data-ttu-id="a4a6b-117">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a4a6b-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4a6b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a4a6b-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/getMemberGroups

```
## <a name="request-headers"></a><span data-ttu-id="a4a6b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a4a6b-119">Request headers</span></span>
| <span data-ttu-id="a4a6b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="a4a6b-120">Name</span></span>       | <span data-ttu-id="a4a6b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4a6b-121">Type</span></span> | <span data-ttu-id="a4a6b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4a6b-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a4a6b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a4a6b-123">Authorization</span></span>  | <span data-ttu-id="a4a6b-124">string</span><span class="sxs-lookup"><span data-stu-id="a4a6b-124">string</span></span>  | <span data-ttu-id="a4a6b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a4a6b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a4a6b-127">Request body</span></span>
<span data-ttu-id="a4a6b-128">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a4a6b-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a4a6b-129">Parameter</span></span>    | <span data-ttu-id="a4a6b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a4a6b-130">Type</span></span>   |<span data-ttu-id="a4a6b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a4a6b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4a6b-132">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a4a6b-132">securityEnabledOnly</span></span>|<span data-ttu-id="a4a6b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="a4a6b-133">Boolean</span></span>|<span data-ttu-id="a4a6b-p105">Defina como **false**. Há suporte para retornar somente os grupos de segurança habilitados apenas para usuários.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-p105">Set to **false**. Returning only security-enabled groups is supported for users only.</span></span>|

## <a name="response"></a><span data-ttu-id="a4a6b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4a6b-136">Response</span></span>

<span data-ttu-id="a4a6b-137">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-137">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4a6b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a4a6b-138">Example</span></span>
<span data-ttu-id="a4a6b-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a4a6b-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a4a6b-140">Request</span></span>
<span data-ttu-id="a4a6b-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-141">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="a4a6b-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a4a6b-142">Response</span></span>
<span data-ttu-id="a4a6b-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a4a6b-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/serviceprincipal-getmembergroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
