---
title: Criar contrato
description: Crie um novo objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 5040651e032a4f5d0ef2340646f11eb51bfff5eb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514422"
---
# <a name="create-agreement"></a><span data-ttu-id="bed90-103">Criar contrato</span><span class="sxs-lookup"><span data-stu-id="bed90-103">Create agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bed90-104">Crie um novo objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="bed90-104">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="bed90-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bed90-105">Permissions</span></span>
<span data-ttu-id="bed90-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed90-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bed90-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bed90-108">Permission type</span></span>                        | <span data-ttu-id="bed90-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bed90-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bed90-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bed90-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bed90-111">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bed90-111">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="bed90-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bed90-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bed90-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bed90-113">Not supported.</span></span> |
|<span data-ttu-id="bed90-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bed90-114">Application</span></span>                            | <span data-ttu-id="bed90-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bed90-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bed90-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bed90-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="bed90-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bed90-117">Request headers</span></span>
| <span data-ttu-id="bed90-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bed90-118">Name</span></span>         | <span data-ttu-id="bed90-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="bed90-119">Type</span></span>        | <span data-ttu-id="bed90-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed90-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="bed90-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="bed90-121">Authorization</span></span> | <span data-ttu-id="bed90-122">string</span><span class="sxs-lookup"><span data-stu-id="bed90-122">string</span></span> | <span data-ttu-id="bed90-123">Token de portador</span><span class="sxs-lookup"><span data-stu-id="bed90-123">Bearer \{token\}.</span></span> <span data-ttu-id="bed90-124">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bed90-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bed90-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bed90-125">Request body</span></span>
<span data-ttu-id="bed90-126">No corpo da solicitação, fornece uma representação de JSON de objeto do [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="bed90-126">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="bed90-127">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="bed90-127">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="bed90-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bed90-128">Property</span></span>     | <span data-ttu-id="bed90-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="bed90-129">Type</span></span>        | <span data-ttu-id="bed90-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed90-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bed90-131">displayName</span><span class="sxs-lookup"><span data-stu-id="bed90-131">displayName</span></span>|<span data-ttu-id="bed90-132">String</span><span class="sxs-lookup"><span data-stu-id="bed90-132">String</span></span>|<span data-ttu-id="bed90-133">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="bed90-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="bed90-134">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="bed90-134">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="bed90-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="bed90-135">Boolean</span></span>|<span data-ttu-id="bed90-136">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="bed90-136">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="bed90-137">arquivos/nome de arquivo</span><span class="sxs-lookup"><span data-stu-id="bed90-137">files/fileName</span></span>|<span data-ttu-id="bed90-138">String</span><span class="sxs-lookup"><span data-stu-id="bed90-138">String</span></span>|<span data-ttu-id="bed90-139">Nome do arquivo contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="bed90-139">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="bed90-140">arquivos/isDefault</span><span class="sxs-lookup"><span data-stu-id="bed90-140">files/isDefault</span></span>|<span data-ttu-id="bed90-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="bed90-141">Boolean</span></span>|<span data-ttu-id="bed90-142">Indica se esse é o arquivo de contrato padrão se nenhum da cultura corresponder a preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="bed90-142">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="bed90-143">Se nenhum do arquivo é marcado como padrão, primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="bed90-143">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="bed90-144">arquivos/idioma</span><span class="sxs-lookup"><span data-stu-id="bed90-144">files/language</span></span>|<span data-ttu-id="bed90-145">String</span><span class="sxs-lookup"><span data-stu-id="bed90-145">String</span></span>|<span data-ttu-id="bed90-146">Cultura do arquivo no formato languagecode2-país/regioncode2 contrato.</span><span class="sxs-lookup"><span data-stu-id="bed90-146">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="bed90-147">languagecode2 é um código de duas letras minúsculas, derivado do ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="bed90-147">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="bed90-148">País/regioncode2 é derivado do ISO 3166 e normalmente consiste em duas letras maiusculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="bed90-148">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="bed90-149">arquivos/fileData/dados</span><span class="sxs-lookup"><span data-stu-id="bed90-149">files/fileData/data</span></span>|<span data-ttu-id="bed90-150">Binária</span><span class="sxs-lookup"><span data-stu-id="bed90-150">Binary</span></span>|<span data-ttu-id="bed90-151">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="bed90-151">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="bed90-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed90-152">Response</span></span>
<span data-ttu-id="bed90-153">Se tiver êxito, este método retornará um `201, Created` objeto de [contrato](../resources/agreement.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bed90-153">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bed90-154">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bed90-154">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bed90-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bed90-155">Request</span></span>
<span data-ttu-id="bed90-156">No corpo da solicitação, fornece uma representação JSON do objeto [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="bed90-156">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="bed90-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed90-157">Response</span></span>
><span data-ttu-id="bed90-p105">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bed90-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/agreement-post-agreements.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
