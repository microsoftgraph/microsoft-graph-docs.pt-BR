---
title: 'informationProtectionLabel: evaluateRemoval'
description: Avaliar qual rótulo remover e como removê-lo com base nas informações de conteúdo existentes.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d01493d122f1e5e632ac0bc90ad5874a25d9eb66
ms.sourcegitcommit: 22d99624036ceaeb1b612538d5196faaa743881f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2020
ms.locfileid: "48932437"
---
# <a name="informationprotectionlabel-evaluateremoval"></a><span data-ttu-id="bd01e-103">informationProtectionLabel: evaluateRemoval</span><span class="sxs-lookup"><span data-stu-id="bd01e-103">informationProtectionLabel: evaluateRemoval</span></span>

<span data-ttu-id="bd01e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd01e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd01e-105">Indique o aplicativo de consumo que ações deve executar para remover as informações de rótulo.</span><span class="sxs-lookup"><span data-stu-id="bd01e-105">Indicate to the consuming application what actions it should take to remove the label information.</span></span>

<span data-ttu-id="bd01e-106">Dada [contentInfo](../resources/contentinfo.md) como uma entrada, que inclui [pares de chave/valor](../resources/keyvaluepair.md)de metadados de conteúdo existentes, a API retorna um [informationProtectionAction](../resources/informationprotectionaction.md) que contém alguma combinação de uma ou mais das seguintes opções:</span><span class="sxs-lookup"><span data-stu-id="bd01e-106">Given [contentInfo](../resources/contentinfo.md) as an input, which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), the API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains some combination of one of more of the following:</span></span> 

* [<span data-ttu-id="bd01e-107">justifyaction</span><span class="sxs-lookup"><span data-stu-id="bd01e-107">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="bd01e-108">metadataaction</span><span class="sxs-lookup"><span data-stu-id="bd01e-108">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="bd01e-109">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="bd01e-109">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="bd01e-110">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="bd01e-110">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="bd01e-111">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="bd01e-111">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="bd01e-112">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="bd01e-112">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="bd01e-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="bd01e-113">Permissions</span></span>

<span data-ttu-id="bd01e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bd01e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd01e-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bd01e-116">Permission type</span></span>                        | <span data-ttu-id="bd01e-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bd01e-117">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bd01e-118">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bd01e-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd01e-119">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="bd01e-119">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="bd01e-120">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bd01e-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd01e-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bd01e-121">Not supported.</span></span>                              |
| <span data-ttu-id="bd01e-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bd01e-122">Application</span></span>                            | <span data-ttu-id="bd01e-123">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd01e-123">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="bd01e-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bd01e-124">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationProtection/policy/labels/evaluateRemoval
```

## <a name="request-headers"></a><span data-ttu-id="bd01e-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bd01e-125">Request headers</span></span>

| <span data-ttu-id="bd01e-126">Nome</span><span class="sxs-lookup"><span data-stu-id="bd01e-126">Name</span></span>          | <span data-ttu-id="bd01e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd01e-127">Description</span></span>                                                                                                                                                                       |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bd01e-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="bd01e-128">Authorization</span></span> | <span data-ttu-id="bd01e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd01e-p102">Bearer {token}. Required.</span></span>                                                                                                                                                         |
| <span data-ttu-id="bd01e-131">Content-type</span><span class="sxs-lookup"><span data-stu-id="bd01e-131">Content-type</span></span>  | <span data-ttu-id="bd01e-p103">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bd01e-p103">application/json. Required.</span></span>                                                                                                                                                       |
| <span data-ttu-id="bd01e-134">User-Agent</span><span class="sxs-lookup"><span data-stu-id="bd01e-134">User-Agent</span></span>    | <span data-ttu-id="bd01e-135">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="bd01e-135">Describes the name and version of the calling application.</span></span> <span data-ttu-id="bd01e-136">Os detalhes surgirão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="bd01e-136">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="bd01e-137">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="bd01e-137">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="bd01e-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bd01e-138">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bd01e-139">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bd01e-139">Request body</span></span>

<span data-ttu-id="bd01e-140">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd01e-140">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="bd01e-141">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bd01e-141">Parameter</span></span>              | <span data-ttu-id="bd01e-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="bd01e-142">Type</span></span>                                                             | <span data-ttu-id="bd01e-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="bd01e-143">Description</span></span>                                                                                                                         |
| :--------------------- | :--------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="bd01e-144">contentInfo</span><span class="sxs-lookup"><span data-stu-id="bd01e-144">contentInfo</span></span>            | [<span data-ttu-id="bd01e-145">contentInfo</span><span class="sxs-lookup"><span data-stu-id="bd01e-145">contentInfo</span></span>](../resources/contentinfo.md)                       | <span data-ttu-id="bd01e-146">Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="bd01e-146">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span> |
| <span data-ttu-id="bd01e-147">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="bd01e-147">downgradeJustification</span></span> | [<span data-ttu-id="bd01e-148">downgradeJustification</span><span class="sxs-lookup"><span data-stu-id="bd01e-148">downgradeJustification</span></span>](../resources/downgradejustification.md) | <span data-ttu-id="bd01e-149">Justificativa que deve ser fornecida pelo usuário ou pela lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="bd01e-149">Justification that must be provided by the user or application logic.</span></span>                                                               |


## <a name="response"></a><span data-ttu-id="bd01e-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd01e-150">Response</span></span>

<span data-ttu-id="bd01e-151">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto da coleção [informationProtectionAction](../resources/informationprotectionaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bd01e-151">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span> <span data-ttu-id="bd01e-152">O [objeto informationProtectionAction](../resources/informationprotectionaction.md) conterá um objeto [metadataaction](../resources/metadataaction.md) que informa ao aplicativo quais metadados serão removidos.</span><span class="sxs-lookup"><span data-stu-id="bd01e-152">The [informationProtectionAction object](../resources/informationprotectionaction.md) will contain a [metadataAction](../resources/metadataaction.md) object that informs the application which metadata to remove.</span></span> 

## <a name="examples"></a><span data-ttu-id="bd01e-153">Exemplos</span><span class="sxs-lookup"><span data-stu-id="bd01e-153">Examples</span></span>

<span data-ttu-id="bd01e-154">Veja a seguir um exemplo de como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="bd01e-154">The following is an example of how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="bd01e-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bd01e-155">Request</span></span>

<span data-ttu-id="bd01e-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="bd01e-156">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="bd01e-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd01e-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateremoval"
}-->

```http
POST https://graph.microsoft.com/beta/informationProtection/policy/labels/evaluateRemoval
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
        "value": "General"
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
  },
  "downgradeJustification": {
        "justificationMessage": "The information has been declassified.",
        "isDowngradeJustified": true
    }
}
```
# <a name="c"></a>[<span data-ttu-id="bd01e-158">C#</span><span class="sxs-lookup"><span data-stu-id="bd01e-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateremoval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bd01e-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd01e-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateremoval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bd01e-160">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd01e-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateremoval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bd01e-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="bd01e-161">Response</span></span>

<span data-ttu-id="bd01e-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="bd01e-162">The following is an example of the response.</span></span>

> <span data-ttu-id="bd01e-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bd01e-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtectionAction",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.informationProtectionAction)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.metadataAction",
            "metadataToRemove": [
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
                "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId"
            ],
            "metadataToAdd": []
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateRemoval",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


