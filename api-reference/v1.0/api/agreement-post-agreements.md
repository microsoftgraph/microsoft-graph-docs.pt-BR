---
title: Criar contrato
description: Crie um novo objeto de contrato.
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: a34d2d78964ca4d50496cfe0850d2ee840f3f04b
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722519"
---
# <a name="create-agreement"></a><span data-ttu-id="ea5ba-103">Criar contrato</span><span class="sxs-lookup"><span data-stu-id="ea5ba-103">Create agreement</span></span>

<span data-ttu-id="ea5ba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea5ba-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ea5ba-105">Crie um novo [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-105">Create a new [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea5ba-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ea5ba-106">Permissions</span></span>
<span data-ttu-id="ea5ba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea5ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea5ba-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ea5ba-109">Permission type</span></span>                        | <span data-ttu-id="ea5ba-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ea5ba-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea5ba-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ea5ba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ea5ba-112">Agreement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea5ba-112">Agreement.ReadWrite.All</span></span> |
|<span data-ttu-id="ea5ba-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ea5ba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea5ba-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-114">Not supported.</span></span> |
|<span data-ttu-id="ea5ba-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ea5ba-115">Application</span></span>                            | <span data-ttu-id="ea5ba-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea5ba-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ea5ba-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/termsOfUse/agreements
```
## <a name="request-headers"></a><span data-ttu-id="ea5ba-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ea5ba-118">Request headers</span></span>
| <span data-ttu-id="ea5ba-119">Nome</span><span class="sxs-lookup"><span data-stu-id="ea5ba-119">Name</span></span>         | <span data-ttu-id="ea5ba-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea5ba-120">Description</span></span> |
|:-------------|:------------|
| <span data-ttu-id="ea5ba-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="ea5ba-121">Authorization</span></span> | <span data-ttu-id="ea5ba-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-122">Bearer \{token\}.</span></span> <span data-ttu-id="ea5ba-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-123">Required.</span></span> |
| <span data-ttu-id="ea5ba-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="ea5ba-124">Content-type</span></span>  | <span data-ttu-id="ea5ba-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea5ba-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ea5ba-127">Request body</span></span>
<span data-ttu-id="ea5ba-128">No corpo da solicitação, fornece uma representação JSON de um [objeto de](../resources/agreement.md) contrato.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-128">In the request body, supply a JSON representation of an [agreement](../resources/agreement.md) object.</span></span>

<span data-ttu-id="ea5ba-129">A tabela a seguir mostra as propriedades que são necessárias ao criar um contrato.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-129">The following table shows the properties that are required when you create an agreement.</span></span>

| <span data-ttu-id="ea5ba-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea5ba-130">Property</span></span>     | <span data-ttu-id="ea5ba-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea5ba-131">Type</span></span>        | <span data-ttu-id="ea5ba-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea5ba-132">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ea5ba-133">displayName</span><span class="sxs-lookup"><span data-stu-id="ea5ba-133">displayName</span></span>|<span data-ttu-id="ea5ba-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea5ba-134">String</span></span>|<span data-ttu-id="ea5ba-135">Nome de exibição do contrato.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-135">Display name of the agreement.</span></span>|
|<span data-ttu-id="ea5ba-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="ea5ba-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="ea5ba-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="ea5ba-137">Boolean</span></span>|<span data-ttu-id="ea5ba-138">Indica se o usuário precisa expandir e exibir o contrato antes de aceitar.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|
|<span data-ttu-id="ea5ba-139">fileName</span><span class="sxs-lookup"><span data-stu-id="ea5ba-139">fileName</span></span>|<span data-ttu-id="ea5ba-140">String</span><span class="sxs-lookup"><span data-stu-id="ea5ba-140">String</span></span>|<span data-ttu-id="ea5ba-141">Nome do arquivo de contrato (por exemplo, TOU.pdf).</span><span class="sxs-lookup"><span data-stu-id="ea5ba-141">Name of the agreement file (for example, TOU.pdf).</span></span>|
|<span data-ttu-id="ea5ba-142">isDefault</span><span class="sxs-lookup"><span data-stu-id="ea5ba-142">isDefault</span></span>|<span data-ttu-id="ea5ba-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="ea5ba-143">Boolean</span></span>|<span data-ttu-id="ea5ba-144">Indica se esse é o arquivo de contrato padrão se o idioma corresponde à preferência do cliente.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-144">Indicates whether this is the default agreement file if the language matches the client preference.</span></span> <span data-ttu-id="ea5ba-145">Se nenhum dos arquivos for marcado como padrão, o primeiro será tratado como padrão.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-145">If none of the files are marked as default, the first one is treated as default.</span></span>|
|<span data-ttu-id="ea5ba-146">idioma</span><span class="sxs-lookup"><span data-stu-id="ea5ba-146">language</span></span>|<span data-ttu-id="ea5ba-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea5ba-147">String</span></span>|<span data-ttu-id="ea5ba-148">O idioma do arquivo de contrato no formato languagecode2-country/regioncode2.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-148">The language of the agreement file in the format languagecode2-country/regioncode2.</span></span> <span data-ttu-id="ea5ba-149">languagecode2 é um código de duas letras minúsculo derivado da ISO 639-1.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-149">languagecode2 is a lowercase two-letter code derived from ISO 639-1.</span></span> <span data-ttu-id="ea5ba-150">country/regioncode2 é derivado da ISO 3166 e geralmente consiste em duas letras maiúsculas, ou uma marca de idioma BCP-47 (por exemplo, en-US).</span><span class="sxs-lookup"><span data-stu-id="ea5ba-150">country/regioncode2 is derived from ISO 3166 and usually consists of two uppercase letters, or a BCP-47 language tag (for example, en-US).</span></span>|
|<span data-ttu-id="ea5ba-151">data</span><span class="sxs-lookup"><span data-stu-id="ea5ba-151">data</span></span>|<span data-ttu-id="ea5ba-152">Binária</span><span class="sxs-lookup"><span data-stu-id="ea5ba-152">Binary</span></span>|<span data-ttu-id="ea5ba-153">Dados que representam os termos de uso do documento PDF.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-153">Data that represents the terms of use for the PDF document.</span></span>|

## <a name="response"></a><span data-ttu-id="ea5ba-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea5ba-154">Response</span></span>
<span data-ttu-id="ea5ba-155">Se tiver êxito, este método retornará `201, Created` um código de resposta e um objeto [agreement](../resources/agreement.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-155">If successful, this method returns a `201, Created` response code and an [agreement](../resources/agreement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea5ba-156">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ea5ba-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea5ba-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ea5ba-157">Request</span></span>
<span data-ttu-id="ea5ba-158">No corpo da solicitação, fornece uma representação JSON do [objeto agreement.](../resources/agreement.md)</span><span class="sxs-lookup"><span data-stu-id="ea5ba-158">In the request body, supply a JSON representation of the [agreement](../resources/agreement.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_agreement_from_agreements"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/termsOfUse/agreements
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


### <a name="response"></a><span data-ttu-id="ea5ba-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="ea5ba-159">Response</span></span>
><span data-ttu-id="ea5ba-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ea5ba-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "093b947f-8363-4979-a47d-4c52b33ee1be"
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


