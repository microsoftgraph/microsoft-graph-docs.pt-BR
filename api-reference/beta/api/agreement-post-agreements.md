---
title: Criar contrato
description: Crie um novo objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: c62fc34d83f8602cb0da56027e4def5d2d904e7e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771208"
---
# <a name="create-agreement"></a><span data-ttu-id="6b5ad-103">Criar contrato</span><span class="sxs-lookup"><span data-stu-id="6b5ad-103">Create agreement</span></span>

<span data-ttu-id="6b5ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b5ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b5ad-105">Crie um novo [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6b5ad-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6b5ad-106">Permissions</span></span>
<span data-ttu-id="6b5ad-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6b5ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b5ad-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6b5ad-109">Permission type</span></span>                        | <span data-ttu-id="6b5ad-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6b5ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b5ad-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6b5ad-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b5ad-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b5ad-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="6b5ad-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6b5ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b5ad-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-114">Not supported.</span></span> |
|<span data-ttu-id="6b5ad-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6b5ad-115">Application</span></span>                            | <span data-ttu-id="6b5ad-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6b5ad-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="6b5ad-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5ad-118">Request headers</span></span>
| <span data-ttu-id="6b5ad-119">Nome</span><span class="sxs-lookup"><span data-stu-id="6b5ad-119">Name</span></span>         | <span data-ttu-id="6b5ad-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b5ad-120">Type</span></span>        | <span data-ttu-id="6b5ad-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b5ad-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="6b5ad-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="6b5ad-122">Authorization</span></span> | <span data-ttu-id="6b5ad-123">string</span><span class="sxs-lookup"><span data-stu-id="6b5ad-123">string</span></span> | <span data-ttu-id="6b5ad-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6b5ad-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5ad-126">Request body</span></span>
<span data-ttu-id="6b5ad-127">No corpo da solicitação, fornece uma representação JSON do [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="6b5ad-127">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="6b5ad-128">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-128">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="6b5ad-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b5ad-129">Property</span></span>     | <span data-ttu-id="6b5ad-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b5ad-130">Type</span></span>        | <span data-ttu-id="6b5ad-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b5ad-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b5ad-132">displayName</span><span class="sxs-lookup"><span data-stu-id="6b5ad-132">displayName</span></span>|<span data-ttu-id="6b5ad-133">String</span><span class="sxs-lookup"><span data-stu-id="6b5ad-133">String</span></span>|<span data-ttu-id="6b5ad-134">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="6b5ad-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="6b5ad-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="6b5ad-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b5ad-136">Boolean</span></span>|<span data-ttu-id="6b5ad-137">Indica se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-137">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="6b5ad-138">files/fileName</span><span class="sxs-lookup"><span data-stu-id="6b5ad-138">files/fileName</span></span>|<span data-ttu-id="6b5ad-139">String</span><span class="sxs-lookup"><span data-stu-id="6b5ad-139">String</span></span>|<span data-ttu-id="6b5ad-140">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="6b5ad-140">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="6b5ad-141">files/isDefault</span><span class="sxs-lookup"><span data-stu-id="6b5ad-141">files/isDefault</span></span>|<span data-ttu-id="6b5ad-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b5ad-142">Boolean</span></span>|<span data-ttu-id="6b5ad-143">Indica se esse é o arquivo de contrato padrão se nenhuma cultura corresponde à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-143">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="6b5ad-144">Se nenhum arquivo for marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-144">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="6b5ad-145">files/language</span><span class="sxs-lookup"><span data-stu-id="6b5ad-145">files/language</span></span>|<span data-ttu-id="6b5ad-146">String</span><span class="sxs-lookup"><span data-stu-id="6b5ad-146">String</span></span>|<span data-ttu-id="6b5ad-147">Cultura do arquivo de contrato no formato languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-147">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="6b5ad-148">languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-148">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="6b5ad-149">country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="6b5ad-149">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="6b5ad-150">files/fileData/data</span><span class="sxs-lookup"><span data-stu-id="6b5ad-150">files/fileData/data</span></span>|<span data-ttu-id="6b5ad-151">Binária</span><span class="sxs-lookup"><span data-stu-id="6b5ad-151">Binary</span></span>|<span data-ttu-id="6b5ad-152">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-152">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="6b5ad-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b5ad-153">Response</span></span>
<span data-ttu-id="6b5ad-154">Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-154">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b5ad-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6b5ad-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6b5ad-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6b5ad-156">Request</span></span>
<span data-ttu-id="6b5ad-157">No corpo da solicitação, fornece uma representação JSON do [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="6b5ad-157">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>



# <a name="http"></a>[<span data-ttu-id="6b5ad-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b5ad-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="6b5ad-159">C#</span><span class="sxs-lookup"><span data-stu-id="6b5ad-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6b5ad-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b5ad-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6b5ad-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b5ad-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6b5ad-162">Java</span><span class="sxs-lookup"><span data-stu-id="6b5ad-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-agreement-from-agreements-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



##### <a name="response"></a><span data-ttu-id="6b5ad-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="6b5ad-163">Response</span></span>
><span data-ttu-id="6b5ad-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6b5ad-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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


