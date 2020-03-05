---
title: Criar contrato
description: Criar um novo objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 1e5a4a836916530589a423b2826eb05805cd04a1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441645"
---
# <a name="create-agreement"></a><span data-ttu-id="7a69e-103">Criar contrato</span><span class="sxs-lookup"><span data-stu-id="7a69e-103">Create agreement</span></span>

<span data-ttu-id="7a69e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7a69e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a69e-105">Criar um novo objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="7a69e-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="7a69e-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7a69e-106">Permissions</span></span>
<span data-ttu-id="7a69e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7a69e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a69e-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7a69e-109">Permission type</span></span>                        | <span data-ttu-id="7a69e-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7a69e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a69e-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7a69e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a69e-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a69e-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="7a69e-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7a69e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a69e-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a69e-114">Not supported.</span></span> |
|<span data-ttu-id="7a69e-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a69e-115">Application</span></span>                            | <span data-ttu-id="7a69e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7a69e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a69e-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7a69e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="7a69e-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7a69e-118">Request headers</span></span>
| <span data-ttu-id="7a69e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="7a69e-119">Name</span></span>         | <span data-ttu-id="7a69e-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a69e-120">Type</span></span>        | <span data-ttu-id="7a69e-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a69e-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7a69e-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7a69e-122">Authorization</span></span> | <span data-ttu-id="7a69e-123">string</span><span class="sxs-lookup"><span data-stu-id="7a69e-123">string</span></span> | <span data-ttu-id="7a69e-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7a69e-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a69e-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7a69e-126">Request body</span></span>
<span data-ttu-id="7a69e-127">No corpo da solicitação, forneça uma representação JSON do objeto [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="7a69e-127">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="7a69e-128">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="7a69e-128">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="7a69e-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a69e-129">Property</span></span>     | <span data-ttu-id="7a69e-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a69e-130">Type</span></span>        | <span data-ttu-id="7a69e-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a69e-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="7a69e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="7a69e-132">displayName</span></span>|<span data-ttu-id="7a69e-133">String</span><span class="sxs-lookup"><span data-stu-id="7a69e-133">String</span></span>|<span data-ttu-id="7a69e-134">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="7a69e-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="7a69e-135">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="7a69e-135">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="7a69e-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a69e-136">Boolean</span></span>|<span data-ttu-id="7a69e-137">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="7a69e-137">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="7a69e-138">arquivos/nome de arquivo</span><span class="sxs-lookup"><span data-stu-id="7a69e-138">files/fileName</span></span>|<span data-ttu-id="7a69e-139">String</span><span class="sxs-lookup"><span data-stu-id="7a69e-139">String</span></span>|<span data-ttu-id="7a69e-140">Nome do arquivo de contrato (por exemplo, TOU. pdf).</span><span class="sxs-lookup"><span data-stu-id="7a69e-140">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="7a69e-141">arquivos/IsDefault</span><span class="sxs-lookup"><span data-stu-id="7a69e-141">files/isDefault</span></span>|<span data-ttu-id="7a69e-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="7a69e-142">Boolean</span></span>|<span data-ttu-id="7a69e-143">Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="7a69e-143">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="7a69e-144">Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="7a69e-144">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="7a69e-145">arquivos/idioma</span><span class="sxs-lookup"><span data-stu-id="7a69e-145">files/language</span></span>|<span data-ttu-id="7a69e-146">String</span><span class="sxs-lookup"><span data-stu-id="7a69e-146">String</span></span>|<span data-ttu-id="7a69e-147">Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="7a69e-147">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="7a69e-148">languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="7a69e-148">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="7a69e-149">Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="7a69e-149">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="7a69e-150">arquivos/fileData/dados</span><span class="sxs-lookup"><span data-stu-id="7a69e-150">files/fileData/data</span></span>|<span data-ttu-id="7a69e-151">Binária</span><span class="sxs-lookup"><span data-stu-id="7a69e-151">Binary</span></span>|<span data-ttu-id="7a69e-152">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="7a69e-152">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="7a69e-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a69e-153">Response</span></span>
<span data-ttu-id="7a69e-154">Se bem-sucedido, este método retorna um `201, Created` código de resposta e um objeto [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7a69e-154">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a69e-155">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7a69e-155">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a69e-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7a69e-156">Request</span></span>
<span data-ttu-id="7a69e-157">No corpo da solicitação, forneça uma representação JSON do objeto [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="7a69e-157">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>


# <a name="http"></a>[<span data-ttu-id="7a69e-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="7a69e-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/beta/agreements
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
# <a name="c"></a>[<span data-ttu-id="7a69e-159">C#</span><span class="sxs-lookup"><span data-stu-id="7a69e-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7a69e-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7a69e-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7a69e-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7a69e-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7a69e-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="7a69e-162">Response</span></span>
><span data-ttu-id="7a69e-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7a69e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
