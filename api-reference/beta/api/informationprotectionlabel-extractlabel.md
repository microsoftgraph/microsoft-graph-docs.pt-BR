---
title: 'informationProtectionLabel: extractLabel'
description: Recupere informationProtectionContentLabel usando metadados de um objeto rotulado.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 043b82820418915f4e38aab1839fee6113b423ec
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994404"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="458d4-103">informationProtectionLabel: extractLabel</span><span class="sxs-lookup"><span data-stu-id="458d4-103">informationProtectionLabel: extractLabel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="458d4-104">Usando os metadados que existem em uma informação já rotulada, resolva os metadados para um rótulo de confidencialidade específico.</span><span class="sxs-lookup"><span data-stu-id="458d4-104">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="458d4-105">A entrada [contentInfo](../resources/contentinfo.md) é resolvida como [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span><span class="sxs-lookup"><span data-stu-id="458d4-105">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="458d4-106">O recurso **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** representa um rótulo de confidencialidade que foi aplicado a uma informação.</span><span class="sxs-lookup"><span data-stu-id="458d4-106">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="458d4-107">os objetos [informationProtectionLabel](../resources/informationprotectionlabel.md) são os rótulos abstratos que fazem parte da política de rótulo de organização e podem ser aplicados às informações.</span><span class="sxs-lookup"><span data-stu-id="458d4-107">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="458d4-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="458d4-108">Permissions</span></span>

<span data-ttu-id="458d4-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="458d4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="458d4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="458d4-111">Permission type</span></span>                        | <span data-ttu-id="458d4-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="458d4-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="458d4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="458d4-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="458d4-114">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="458d4-114">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="458d4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="458d4-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="458d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="458d4-116">Not supported.</span></span>                              |
| <span data-ttu-id="458d4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="458d4-117">Application</span></span>                            | <span data-ttu-id="458d4-118">InformationProtectionPolicy. Read. All</span><span class="sxs-lookup"><span data-stu-id="458d4-118">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="458d4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="458d4-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="458d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="458d4-120">Request headers</span></span>

| <span data-ttu-id="458d4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="458d4-121">Name</span></span>          | <span data-ttu-id="458d4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="458d4-122">Description</span></span>                    |
| :------------ | :----------------------------- |
| <span data-ttu-id="458d4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="458d4-123">Authorization</span></span> | <span data-ttu-id="458d4-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="458d4-p104">Bearer {token}. Required.</span></span>                 |
| <span data-ttu-id="458d4-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="458d4-126">Content-type</span></span>  | <span data-ttu-id="458d4-127">Content-Type: Application/JSON.</span><span class="sxs-lookup"><span data-stu-id="458d4-127">Content-type: application/json.</span></span> <span data-ttu-id="458d4-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="458d4-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="458d4-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="458d4-129">Request body</span></span>

<span data-ttu-id="458d4-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="458d4-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="458d4-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="458d4-131">Parameter</span></span>   | <span data-ttu-id="458d4-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="458d4-132">Type</span></span>                                       | <span data-ttu-id="458d4-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="458d4-133">Description</span></span>                                                                                                                                                                                                   |
| :---------- | :----------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="458d4-134">contentInfo</span><span class="sxs-lookup"><span data-stu-id="458d4-134">contentInfo</span></span> | [<span data-ttu-id="458d4-135">contentInfo</span><span class="sxs-lookup"><span data-stu-id="458d4-135">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="458d4-136">Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="458d4-136">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="458d4-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="458d4-137">Response</span></span>

<span data-ttu-id="458d4-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e um novo objeto [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="458d4-138">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="458d4-139">Exemplos</span><span class="sxs-lookup"><span data-stu-id="458d4-139">Examples</span></span>

<span data-ttu-id="458d4-140">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="458d4-140">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="458d4-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="458d4-141">Request</span></span>

<span data-ttu-id="458d4-142">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="458d4-142">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="458d4-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="458d4-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/extractLabel
Content-type: application/json

{
    "contentInfo": {
        "@odata.type": "#microsoft.graph.contentInfo",
        "format@odata.type": "#microsoft.graph.contentFormat",
        "format": "default",
        "identifier": null,
        "state@odata.type": "#microsoft.graph.contentState",
        "state": "rest",
        "metadata@odata.type": "#Collection(microsoft.graph.keyValuePair)",
        "metadata": [
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                "value": "True"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                "value": "Standard"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                "value": "1/1/0001 12:00:00 AM"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                "value": "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                "value": "Top Secret"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                "value": "0"
            },
            {
                "@odata.type": "#microsoft.graph.keyValuePair",
                "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
                "value": "00000000-0000-0000-0000-000000000000"
            }
        ]
    }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="458d4-144">C#</span><span class="sxs-lookup"><span data-stu-id="458d4-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="458d4-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="458d4-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="458d4-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="458d4-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="458d4-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="458d4-147">Response</span></span>

<span data-ttu-id="458d4-148">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="458d4-148">The following is an example of the response.</span></span>

> <span data-ttu-id="458d4-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="458d4-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionContentLabel"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.informationProtectionContentLabel",
    "creationDateTime": "1970-01-01T00:00:00Z",
    "assignmentMethod": "standard",
    "label": {
        "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
        "name": "Top Secret",
        "description": "",
        "color": "#000000",
        "sensitivity": 13,
        "tooltip": "This information is top secret.",
        "isActive": true
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: extractLabel",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
