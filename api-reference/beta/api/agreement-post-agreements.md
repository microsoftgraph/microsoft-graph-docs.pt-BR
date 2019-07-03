---
title: Criar contrato
description: Criar um novo objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: caf98c8f5d1f006ce64c6e39c0d2e52cbfbde61a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439788"
---
# <a name="create-agreement"></a><span data-ttu-id="78631-103">Criar contrato</span><span class="sxs-lookup"><span data-stu-id="78631-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78631-104">Criar um novo objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="78631-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="78631-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="78631-105">Permissions</span></span>
<span data-ttu-id="78631-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78631-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78631-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78631-108">Permission type</span></span>                        | <span data-ttu-id="78631-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="78631-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="78631-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78631-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="78631-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78631-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="78631-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78631-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="78631-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78631-113">Not supported.</span></span> |
|<span data-ttu-id="78631-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78631-114">Application</span></span>                            | <span data-ttu-id="78631-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78631-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="78631-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78631-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="78631-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78631-117">Request headers</span></span>
| <span data-ttu-id="78631-118">Nome</span><span class="sxs-lookup"><span data-stu-id="78631-118">Name</span></span>         | <span data-ttu-id="78631-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="78631-119">Type</span></span>        | <span data-ttu-id="78631-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="78631-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="78631-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="78631-121">Authorization</span></span> | <span data-ttu-id="78631-122">string</span><span class="sxs-lookup"><span data-stu-id="78631-122">string</span></span> | <span data-ttu-id="78631-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78631-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="78631-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78631-125">Request body</span></span>
<span data-ttu-id="78631-126">No corpo da solicitação, forneça uma representação JSON do objeto [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="78631-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="78631-127">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="78631-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="78631-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78631-128">Property</span></span>     | <span data-ttu-id="78631-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="78631-129">Type</span></span>        | <span data-ttu-id="78631-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="78631-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="78631-131">displayName</span><span class="sxs-lookup"><span data-stu-id="78631-131">displayName</span></span>|<span data-ttu-id="78631-132">String</span><span class="sxs-lookup"><span data-stu-id="78631-132">String</span></span>|<span data-ttu-id="78631-133">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="78631-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="78631-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="78631-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="78631-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="78631-135">Boolean</span></span>|<span data-ttu-id="78631-136">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="78631-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="78631-137">arquivos/nome de arquivo</span><span class="sxs-lookup"><span data-stu-id="78631-137">files/fileName</span></span>|<span data-ttu-id="78631-138">String</span><span class="sxs-lookup"><span data-stu-id="78631-138">String</span></span>|<span data-ttu-id="78631-139">Nome do arquivo de contrato (por exemplo, TOU. pdf).</span><span class="sxs-lookup"><span data-stu-id="78631-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="78631-140">arquivos/IsDefault</span><span class="sxs-lookup"><span data-stu-id="78631-140">files/isDefault</span></span>|<span data-ttu-id="78631-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="78631-141">Boolean</span></span>|<span data-ttu-id="78631-142">Indica se este é o arquivo de contrato padrão se nenhuma das culturas corresponder à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="78631-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="78631-143">Se nenhum dos arquivos estiver marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="78631-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="78631-144">arquivos/idioma</span><span class="sxs-lookup"><span data-stu-id="78631-144">files/language</span></span>|<span data-ttu-id="78631-145">String</span><span class="sxs-lookup"><span data-stu-id="78631-145">String</span></span>|<span data-ttu-id="78631-146">Cultura do arquivo de contrato no formato languagecode2-Country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="78631-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="78631-147">languagecode2 é um código de duas letras em minúsculas derivado de ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="78631-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="78631-148">Country/regioncode2 é derivado de ISO 3166 e geralmente consiste em duas letras maiúsculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="78631-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="78631-149">arquivos/fileData/dados</span><span class="sxs-lookup"><span data-stu-id="78631-149">files/fileData/data</span></span>|<span data-ttu-id="78631-150">Binária</span><span class="sxs-lookup"><span data-stu-id="78631-150">Binary</span></span>|<span data-ttu-id="78631-151">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="78631-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="78631-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="78631-152">Response</span></span>
<span data-ttu-id="78631-153">Se bem-sucedido, este método retorna um `201, Created` código de resposta e um objeto [Agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78631-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78631-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78631-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="78631-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78631-155">Request</span></span>
<span data-ttu-id="78631-156">No corpo da solicitação, forneça uma representação JSON do objeto [Agreement](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="78631-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="78631-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="78631-157">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="78631-158">C#</span><span class="sxs-lookup"><span data-stu-id="78631-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-agreement-from-agreements-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="78631-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="78631-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-agreement-from-agreements-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="78631-160">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="78631-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-agreement-from-agreements-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="78631-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="78631-161">Response</span></span>
><span data-ttu-id="78631-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78631-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
