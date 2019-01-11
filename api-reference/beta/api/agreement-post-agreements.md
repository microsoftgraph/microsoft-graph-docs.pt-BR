---
title: Criar contrato
description: Crie um novo objeto de contrato.
localization_priority: Normal
ms.openlocfilehash: 4768912a7c5be722878d6b910d6d68ded460c702
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870634"
---
# <a name="create-agreement"></a><span data-ttu-id="cfb8f-103">Criar contrato</span><span class="sxs-lookup"><span data-stu-id="cfb8f-103">Create agreement</span></span>

> <span data-ttu-id="cfb8f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfb8f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cfb8f-106">Crie um novo objeto de [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="cfb8f-106">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cfb8f-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="cfb8f-107">Permissions</span></span>
<span data-ttu-id="cfb8f-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cfb8f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cfb8f-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cfb8f-110">Permission type</span></span>                        | <span data-ttu-id="cfb8f-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cfb8f-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="cfb8f-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cfb8f-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="cfb8f-113">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cfb8f-113">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="cfb8f-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cfb8f-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cfb8f-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-115">Not supported.</span></span> |
|<span data-ttu-id="cfb8f-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cfb8f-116">Application</span></span>                            | <span data-ttu-id="cfb8f-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cfb8f-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cfb8f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /agreements
```
## <a name="request-headers"></a><span data-ttu-id="cfb8f-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb8f-119">Request headers</span></span>
| <span data-ttu-id="cfb8f-120">Nome</span><span class="sxs-lookup"><span data-stu-id="cfb8f-120">Name</span></span>         | <span data-ttu-id="cfb8f-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfb8f-121">Type</span></span>        | <span data-ttu-id="cfb8f-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb8f-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="cfb8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="cfb8f-123">Authorization</span></span> | <span data-ttu-id="cfb8f-124">string</span><span class="sxs-lookup"><span data-stu-id="cfb8f-124">string</span></span> | <span data-ttu-id="cfb8f-125">Portador \{token\}.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-125">Bearer \{token\}.</span></span> <span data-ttu-id="cfb8f-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cfb8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb8f-127">Request body</span></span>
<span data-ttu-id="cfb8f-128">No corpo da solicitação, fornece uma representação de JSON de objeto do [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="cfb8f-128">In the request body, supply a JSON representation of [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="cfb8f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar um usuário.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-129">The following table shows the properties that are required when you create a user.</span></span>

| <span data-ttu-id="cfb8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cfb8f-130">Property</span></span>     | <span data-ttu-id="cfb8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="cfb8f-131">Type</span></span>        | <span data-ttu-id="cfb8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="cfb8f-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cfb8f-133">displayName</span><span class="sxs-lookup"><span data-stu-id="cfb8f-133">displayName</span></span>|<span data-ttu-id="cfb8f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfb8f-134">String</span></span>|<span data-ttu-id="cfb8f-135">Nome para exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="cfb8f-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="cfb8f-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="cfb8f-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="cfb8f-137">Boolean</span></span>|<span data-ttu-id="cfb8f-138">Indica se o usuário tem que expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="cfb8f-139">arquivos/nome de arquivo</span><span class="sxs-lookup"><span data-stu-id="cfb8f-139">files/fileName</span></span>|<span data-ttu-id="cfb8f-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfb8f-140">String</span></span>|<span data-ttu-id="cfb8f-141">Nome do arquivo contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="cfb8f-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="cfb8f-142">arquivos/isDefault</span><span class="sxs-lookup"><span data-stu-id="cfb8f-142">files/isDefault</span></span>|<span data-ttu-id="cfb8f-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="cfb8f-143">Boolean</span></span>|<span data-ttu-id="cfb8f-144">Indica se esse é o arquivo de contrato padrão se nenhum da cultura corresponder a preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-144">Indicates whether this is the default agreement file if none of the culture matches the client preference.</span></span> <span data-ttu-id="cfb8f-145">Se nenhum do arquivo é marcado como padrão, primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-145">If none of the file is marked as default, the first one will be treated as default.</span></span>|
|<span data-ttu-id="cfb8f-146">arquivos/idioma</span><span class="sxs-lookup"><span data-stu-id="cfb8f-146">files/language</span></span>|<span data-ttu-id="cfb8f-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cfb8f-147">String</span></span>|<span data-ttu-id="cfb8f-148">Cultura do arquivo no formato languagecode2-país/regioncode2 contrato.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-148">Culture of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="cfb8f-149">languagecode2 é um código de duas letras minúsculas, derivado do ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="cfb8f-150">País/regioncode2 é derivado do ISO 3166 e normalmente consiste em duas letras maiusculas ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="cfb8f-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="cfb8f-151">arquivos/fileData/dados</span><span class="sxs-lookup"><span data-stu-id="cfb8f-151">files/fileData/data</span></span>|<span data-ttu-id="cfb8f-152">Binária</span><span class="sxs-lookup"><span data-stu-id="cfb8f-152">Binary</span></span>|<span data-ttu-id="cfb8f-153">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-153">Data representing the terms of use the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="cfb8f-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfb8f-154">Response</span></span>
<span data-ttu-id="cfb8f-155">Se tiver êxito, este método retornará um `201, Created` objeto de [contrato](../resources/agreement.md) e código de resposta no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-155">If successful, this method returns a `201, Created` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cfb8f-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cfb8f-156">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cfb8f-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cfb8f-157">Request</span></span>
<span data-ttu-id="cfb8f-158">No corpo da solicitação, fornece uma representação JSON do objeto [contrato](../resources/agreement.md) .</span><span class="sxs-lookup"><span data-stu-id="cfb8f-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="cfb8f-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="cfb8f-159">Response</span></span>
><span data-ttu-id="cfb8f-p106">\*\*Observação: \*\*o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cfb8f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
