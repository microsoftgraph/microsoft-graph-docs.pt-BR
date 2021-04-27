---
title: Criar contrato
description: Crie um novo objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 53d11dc97d2662906e06b661cd967d5536419a86
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048201"
---
# <a name="create-agreement"></a><span data-ttu-id="9566b-103">Criar contrato</span><span class="sxs-lookup"><span data-stu-id="9566b-103">Create agreement</span></span>

<span data-ttu-id="9566b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9566b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9566b-105">Crie um novo [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="9566b-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9566b-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="9566b-106">Permissions</span></span>
<span data-ttu-id="9566b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9566b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9566b-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9566b-109">Permission type</span></span>                        | <span data-ttu-id="9566b-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9566b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9566b-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9566b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9566b-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9566b-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="9566b-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9566b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9566b-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9566b-114">Not supported.</span></span> |
|<span data-ttu-id="9566b-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9566b-115">Application</span></span>                            | <span data-ttu-id="9566b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9566b-116">Not supported.</span></span> |

<span data-ttu-id="9566b-117">Ao chamar em nome de um usuário, o usuário precisa pertencer a uma das seguintes funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="9566b-117">When calling on behalf of a user, the user needs to belong to one of the following directory roles.</span></span> <span data-ttu-id="9566b-118">Para saber mais sobre funções de diretório, consulte Funções do [Azure AD integrados](/azure/active-directory/roles/permissions-reference):</span><span class="sxs-lookup"><span data-stu-id="9566b-118">To learn more about directory roles, see [Azure AD built-in roles](/azure/active-directory/roles/permissions-reference):</span></span>
+ <span data-ttu-id="9566b-119">Administrador Global</span><span class="sxs-lookup"><span data-stu-id="9566b-119">Global Administrator</span></span>
+ <span data-ttu-id="9566b-120">Administrador de Acesso Condicional</span><span class="sxs-lookup"><span data-stu-id="9566b-120">Conditional Access Administrator</span></span>
+ <span data-ttu-id="9566b-121">Administrador de Segurança</span><span class="sxs-lookup"><span data-stu-id="9566b-121">Security Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="9566b-122">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9566b-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="9566b-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9566b-123">Request headers</span></span>
| <span data-ttu-id="9566b-124">Nome</span><span class="sxs-lookup"><span data-stu-id="9566b-124">Name</span></span>         | <span data-ttu-id="9566b-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="9566b-125">Type</span></span>        | <span data-ttu-id="9566b-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="9566b-126">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="9566b-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="9566b-127">Authorization</span></span> | <span data-ttu-id="9566b-128">string</span><span class="sxs-lookup"><span data-stu-id="9566b-128">string</span></span> | <span data-ttu-id="9566b-p103">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9566b-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9566b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9566b-131">Request body</span></span>
<span data-ttu-id="9566b-132">No corpo da solicitação, fornece uma representação JSON do [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="9566b-132">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="9566b-133">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="9566b-133">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="9566b-134">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9566b-134">Property</span></span>     | <span data-ttu-id="9566b-135">Tipo</span><span class="sxs-lookup"><span data-stu-id="9566b-135">Type</span></span>        | <span data-ttu-id="9566b-136">Descrição</span><span class="sxs-lookup"><span data-stu-id="9566b-136">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9566b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9566b-137">displayName</span></span>|<span data-ttu-id="9566b-138">String</span><span class="sxs-lookup"><span data-stu-id="9566b-138">String</span></span>|<span data-ttu-id="9566b-139">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="9566b-139">Display name of the agreement.</span></span>|
|<span data-ttu-id="9566b-140">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="9566b-140">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="9566b-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="9566b-141">Boolean</span></span>|<span data-ttu-id="9566b-142">Indica se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="9566b-142">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="9566b-143">files/fileName</span><span class="sxs-lookup"><span data-stu-id="9566b-143">files/fileName</span></span>|<span data-ttu-id="9566b-144">String</span><span class="sxs-lookup"><span data-stu-id="9566b-144">String</span></span>|<span data-ttu-id="9566b-145">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="9566b-145">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="9566b-146">files/isDefault</span><span class="sxs-lookup"><span data-stu-id="9566b-146">files/isDefault</span></span>|<span data-ttu-id="9566b-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="9566b-147">Boolean</span></span>|<span data-ttu-id="9566b-148">Indica se esse é o arquivo de contrato padrão se nenhuma cultura corresponde à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="9566b-148">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="9566b-149">Se nenhum arquivo for marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="9566b-149">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="9566b-150">files/language</span><span class="sxs-lookup"><span data-stu-id="9566b-150">files/language</span></span>|<span data-ttu-id="9566b-151">String</span><span class="sxs-lookup"><span data-stu-id="9566b-151">String</span></span>|<span data-ttu-id="9566b-152">Cultura do arquivo de contrato no formato languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="9566b-152">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="9566b-153">languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="9566b-153">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="9566b-154">country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="9566b-154">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="9566b-155">files/fileData/data</span><span class="sxs-lookup"><span data-stu-id="9566b-155">files/fileData/data</span></span>|<span data-ttu-id="9566b-156">Binário</span><span class="sxs-lookup"><span data-stu-id="9566b-156">Binary</span></span>|<span data-ttu-id="9566b-157">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="9566b-157">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="9566b-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="9566b-158">Response</span></span>
<span data-ttu-id="9566b-159">Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="9566b-159">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9566b-160">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9566b-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9566b-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9566b-161">Request</span></span>
<span data-ttu-id="9566b-162">No corpo da solicitação, fornece uma representação JSON do [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="9566b-162">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="9566b-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="9566b-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/termsOfUse/agreements
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "files": [
    {
      "fileName": "TOU.pdf",
      "language": "en",
      "isDefault": true,
      "fileData": {
        "data": "SGVsbG8gd29ybGQ="
      }
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="9566b-164">C#</span><span class="sxs-lookup"><span data-stu-id="9566b-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9566b-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9566b-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9566b-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9566b-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9566b-167">Java</span><span class="sxs-lookup"><span data-stu-id="9566b-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="9566b-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="9566b-168">Response</span></span>
><span data-ttu-id="9566b-169">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="9566b-169">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


