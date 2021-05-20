---
title: 'informationProtectionLabel: extractLabel'
description: Recupere informationProtectionContentLabel usando metadados de um objeto rotulado.
localization_priority: Normal
author: tommoser
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: c0a7012c02132ad2ed46d82e857e8de62be1e746
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579610"
---
# <a name="informationprotectionlabel-extractlabel"></a><span data-ttu-id="3037c-103">informationProtectionLabel: extractLabel</span><span class="sxs-lookup"><span data-stu-id="3037c-103">informationProtectionLabel: extractLabel</span></span>

<span data-ttu-id="3037c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3037c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3037c-105">Usando os metadados existentes em uma informação já rotulada, resolva os metadados para um rótulo de sensibilidade específico.</span><span class="sxs-lookup"><span data-stu-id="3037c-105">Using the metadata that exists on an already-labeled piece of information, resolve the metadata to a specific sensitivity label.</span></span> <span data-ttu-id="3037c-106">A [entrada contentInfo](../resources/contentinfo.md) é resolvida para [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span><span class="sxs-lookup"><span data-stu-id="3037c-106">The [contentInfo](../resources/contentinfo.md) input is resolved to [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md).</span></span>

>[!NOTE]
><span data-ttu-id="3037c-107">O **[recurso informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** representa um rótulo de sensibilidade que foi aplicado a uma informação.</span><span class="sxs-lookup"><span data-stu-id="3037c-107">The **[informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md)** resource represents a sensitivity label that has been applied to a piece of information.</span></span> <span data-ttu-id="3037c-108">[os objetos informationProtectionLabel](../resources/informationprotectionlabel.md) são os rótulos abstratos que fazem parte da política de rotulagem organizacional e podem ser aplicados às informações.</span><span class="sxs-lookup"><span data-stu-id="3037c-108">[informationProtectionLabel](../resources/informationprotectionlabel.md) objects are the abstract labels that are part of the organizational labeling policy and can be applied to information.</span></span>

## <a name="permissions"></a><span data-ttu-id="3037c-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="3037c-109">Permissions</span></span>

<span data-ttu-id="3037c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3037c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3037c-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3037c-112">Permission type</span></span>                        | <span data-ttu-id="3037c-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3037c-113">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="3037c-114">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3037c-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="3037c-115">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="3037c-115">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="3037c-116">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3037c-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3037c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3037c-117">Not supported.</span></span>                              |
| <span data-ttu-id="3037c-118">Application</span><span class="sxs-lookup"><span data-stu-id="3037c-118">Application</span></span>                            | <span data-ttu-id="3037c-119">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="3037c-119">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="3037c-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3037c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/extractLabel
```

## <a name="request-headers"></a><span data-ttu-id="3037c-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3037c-121">Request headers</span></span>

| <span data-ttu-id="3037c-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3037c-122">Name</span></span>          | <span data-ttu-id="3037c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3037c-123">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3037c-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3037c-124">Authorization</span></span> | <span data-ttu-id="3037c-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3037c-p104">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="3037c-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="3037c-127">Content-type</span></span>  | <span data-ttu-id="3037c-128">Tipo de conteúdo: application/json.</span><span class="sxs-lookup"><span data-stu-id="3037c-128">Content-type: application/json.</span></span> <span data-ttu-id="3037c-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3037c-129">Required.</span></span>                                                                                                                                         |
| <span data-ttu-id="3037c-130">User-Agent</span><span class="sxs-lookup"><span data-stu-id="3037c-130">User-Agent</span></span>    | <span data-ttu-id="3037c-131">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="3037c-131">Describes the name and version of the calling application.</span></span> <span data-ttu-id="3037c-132">Os detalhes aparecerão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="3037c-132">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="3037c-133">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="3037c-133">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="3037c-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="3037c-134">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3037c-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3037c-135">Request body</span></span>

<span data-ttu-id="3037c-136">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3037c-136">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="3037c-137">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="3037c-137">Parameter</span></span>   | <span data-ttu-id="3037c-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="3037c-138">Type</span></span>                                       | <span data-ttu-id="3037c-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="3037c-139">Description</span></span>                                                                                                                         |
| :---------- | :----------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="3037c-140">contentInfo</span><span class="sxs-lookup"><span data-stu-id="3037c-140">contentInfo</span></span> | [<span data-ttu-id="3037c-141">contentInfo</span><span class="sxs-lookup"><span data-stu-id="3037c-141">contentInfo</span></span>](../resources/contentinfo.md) | <span data-ttu-id="3037c-142">Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="3037c-142">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |

## <a name="response"></a><span data-ttu-id="3037c-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="3037c-143">Response</span></span>

<span data-ttu-id="3037c-144">Se tiver êxito, este método retornará um código de resposta e um `200 OK` novo [objeto informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3037c-144">If successful, this method returns a `200 OK` response code and a new [informationProtectionContentLabel](../resources/informationprotectioncontentlabel.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3037c-145">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3037c-145">Examples</span></span>

<span data-ttu-id="3037c-146">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="3037c-146">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="3037c-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3037c-147">Request</span></span>

<span data-ttu-id="3037c-148">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3037c-148">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3037c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="3037c-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_extractlabel"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/extractLabel
Content-type: application/json
User-agent: ContosoLOBApp/1.0

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
# <a name="c"></a>[<span data-ttu-id="3037c-150">C#</span><span class="sxs-lookup"><span data-stu-id="3037c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-extractlabel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3037c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3037c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-extractlabel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3037c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3037c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-extractlabel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3037c-153">Java</span><span class="sxs-lookup"><span data-stu-id="3037c-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/informationprotectionlabel-extractlabel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3037c-154">Resposta</span><span class="sxs-lookup"><span data-stu-id="3037c-154">Response</span></span>

<span data-ttu-id="3037c-155">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3037c-155">The following is an example of the response.</span></span>

> <span data-ttu-id="3037c-156">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="3037c-156">**Note:** The response object shown here might be shortened for readability.</span></span>

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
        "isActive": true,
        "parent" : null
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


