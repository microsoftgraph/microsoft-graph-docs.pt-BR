---
title: 'informationProtectionLabel: evaluateClassificationResults'
description: Avaliar qual rótulo aplicar com base nas informações de conteúdo existentes e em um resultado de classificação.
localization_priority: Normal
author: tommoser
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 22fb19a5d44ff9bed091c1cbd84183470a3490ce
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48001461"
---
# <a name="informationprotectionlabel-evaluateclassificationresults"></a><span data-ttu-id="2e9ad-103">informationProtectionLabel: evaluateClassificationResults</span><span class="sxs-lookup"><span data-stu-id="2e9ad-103">informationProtectionLabel: evaluateClassificationResults</span></span>

<span data-ttu-id="2e9ad-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e9ad-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e9ad-105">Usando [os resultados da classificação](../resources/classificationresult.md), calcule o [rótulo de proteção de informações](../resources/informationprotectionlabel.md) que deve ser aplicado e retorne o conjunto de ações que devem ser executadas para rotular corretamente as informações.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-105">Using [classification results](../resources/classificationresult.md), compute the [information protection label](../resources/informationprotectionlabel.md) that should be applied and return the set of actions that must be taken to correctly label the information.</span></span> <span data-ttu-id="2e9ad-106">Essa API é útil quando um rótulo deve ser definido automaticamente com base na classificação do conteúdo do arquivo, em vez de ser rotulado diretamente por um usuário ou serviço.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-106">This API is useful when a label should be set automatically based on classification of the file contents, rather than labeled directly by a user or service.</span></span> 

<span data-ttu-id="2e9ad-107">Para avaliar com base nos resultados da classificação, forneça [contentInfo](../resources/contentinfo.md), que inclui [pares de chave/valor](../resources/keyvaluepair.md)de metadados de conteúdo existentes e [resultados da classificação](../resources/classificationresult.md).</span><span class="sxs-lookup"><span data-stu-id="2e9ad-107">To evaluate based on classification results, provide [contentInfo](../resources/contentinfo.md), which includes existing content metadata [key/value pairs](../resources/keyvaluepair.md), and [classification results](../resources/classificationresult.md).</span></span> <span data-ttu-id="2e9ad-108">A API retorna um [informationProtectionAction](../resources/informationprotectionaction.md) que contém um ou mais dos seguintes itens:</span><span class="sxs-lookup"><span data-stu-id="2e9ad-108">The API returns an [informationProtectionAction](../resources/informationprotectionaction.md) that contains one of more of the following:</span></span> 

* [<span data-ttu-id="2e9ad-109">addContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-109">addContentFooterAction</span></span>](../resources/addcontentfooteraction.md)
* [<span data-ttu-id="2e9ad-110">addContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-110">addContentHeaderAction</span></span>](../resources/addcontentheaderaction.md)
* [<span data-ttu-id="2e9ad-111">addwatermarkaction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-111">addWatermarkAction</span></span>](../resources/addWatermarkaction.md)
* [<span data-ttu-id="2e9ad-112">applyLabelAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-112">applyLabelAction</span></span>](../resources/applylabelaction.md)
* [<span data-ttu-id="2e9ad-113">Personalizada</span><span class="sxs-lookup"><span data-stu-id="2e9ad-113">customAction</span></span>](../resources/customaction.md)
* [<span data-ttu-id="2e9ad-114">justifyaction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-114">justifyAction</span></span>](../resources/justifyaction.md)
* [<span data-ttu-id="2e9ad-115">metadataaction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-115">metadataAction</span></span>](../resources/metadataaction.md)
* [<span data-ttu-id="2e9ad-116">protectAdhocAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-116">protectAdhocAction</span></span>](../resources/protectadhocaction.md)
* [<span data-ttu-id="2e9ad-117">protectByTemplateAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-117">protectByTemplateAction</span></span>](../resources/protectBytemplateaction.md)
* [<span data-ttu-id="2e9ad-118">protectionDoNotForwardAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-118">protectionDoNotForwardAction</span></span>](../resources/protectdonotforwardaction.md)
* [<span data-ttu-id="2e9ad-119">recommendLabelAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-119">recommendLabelAction</span></span>](../resources/recommendlabelaction.md)
* [<span data-ttu-id="2e9ad-120">removeContentFooterAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-120">removeContentFooterAction</span></span>](../resources/removecontentfooteraction.md)
* [<span data-ttu-id="2e9ad-121">removeContentHeaderAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-121">removeContentHeaderAction</span></span>](../resources/removecontentheaderaction.md)
* [<span data-ttu-id="2e9ad-122">removeProtectionAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-122">removeProtectionAction</span></span>](../resources/removeprotectionaction.md)
* [<span data-ttu-id="2e9ad-123">removeWatermarkAction</span><span class="sxs-lookup"><span data-stu-id="2e9ad-123">removeWatermarkAction</span></span>](../resources/removewatermarkaction.md)

## <a name="permissions"></a><span data-ttu-id="2e9ad-124">Permissões</span><span class="sxs-lookup"><span data-stu-id="2e9ad-124">Permissions</span></span>

<span data-ttu-id="2e9ad-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2e9ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2e9ad-127">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2e9ad-127">Permission type</span></span>                        | <span data-ttu-id="2e9ad-128">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2e9ad-128">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="2e9ad-129">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2e9ad-129">Delegated (work or school account)</span></span>     | <span data-ttu-id="2e9ad-130">InformationProtectionPolicy. Read</span><span class="sxs-lookup"><span data-stu-id="2e9ad-130">InformationProtectionPolicy.Read</span></span>            |
| <span data-ttu-id="2e9ad-131">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2e9ad-131">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e9ad-132">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-132">Not supported.</span></span>                              |
| <span data-ttu-id="2e9ad-133">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2e9ad-133">Application</span></span>                            | <span data-ttu-id="2e9ad-134">InformationProtectionPolicy.Read.All</span><span class="sxs-lookup"><span data-stu-id="2e9ad-134">InformationProtectionPolicy.Read.All</span></span>        |

## <a name="http-request"></a><span data-ttu-id="2e9ad-135">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2e9ad-135">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /informationprotection/policy/labels/{id}/evaluateClassificationResults
```

## <a name="request-headers"></a><span data-ttu-id="2e9ad-136">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9ad-136">Request headers</span></span>

| <span data-ttu-id="2e9ad-137">Nome</span><span class="sxs-lookup"><span data-stu-id="2e9ad-137">Name</span></span>          | <span data-ttu-id="2e9ad-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e9ad-138">Description</span></span>                                                                                                                                                           |
| :------------ | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="2e9ad-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="2e9ad-139">Authorization</span></span> | <span data-ttu-id="2e9ad-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-p104">Bearer {token}. Required.</span></span>                                                                                                                                             |
| <span data-ttu-id="2e9ad-142">Content-type</span><span class="sxs-lookup"><span data-stu-id="2e9ad-142">Content-type</span></span>  | <span data-ttu-id="2e9ad-p105">application/json. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-p105">application/json. Required.</span></span>                                                                                                                                           |
| <span data-ttu-id="2e9ad-145">Agente de usuário</span><span class="sxs-lookup"><span data-stu-id="2e9ad-145">User-Agent</span></span>    | <span data-ttu-id="2e9ad-146">Descreve o nome e a versão do aplicativo de chamada.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-146">Describes the name and version of the calling application.</span></span> <span data-ttu-id="2e9ad-147">Os detalhes surgirão no Azure Information Protection Analytics.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-147">Details will surface in Azure Information Protection Analytics.</span></span> <span data-ttu-id="2e9ad-148">O formato sugerido é ApplicationName/Version.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-148">Suggested format is ApplicationName/Version.</span></span> <span data-ttu-id="2e9ad-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-149">Optional.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2e9ad-150">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9ad-150">Request body</span></span>

<span data-ttu-id="2e9ad-151">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-151">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2e9ad-152">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2e9ad-152">Parameter</span></span>             | <span data-ttu-id="2e9ad-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="2e9ad-153">Type</span></span>                                                                    | <span data-ttu-id="2e9ad-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="2e9ad-154">Description</span></span>                                                                                                                                                                                                                                                                           |
| :-------------------- | :---------------------------------------------------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <span data-ttu-id="2e9ad-155">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2e9ad-155">contentInfo</span></span>           | [<span data-ttu-id="2e9ad-156">contentInfo</span><span class="sxs-lookup"><span data-stu-id="2e9ad-156">contentInfo</span></span>](../resources/contentInfo.md)                              | <span data-ttu-id="2e9ad-157">Fornece detalhes sobre o formato de conteúdo, o estado do conteúdo e os [metadados](../resources/keyvaluepair.md) existentes como pares de chave/valor.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-157">Provides details about the content format, content state, and existing [metadata](../resources/keyvaluepair.md) as key/value pairs.</span></span>                                                                                                                                                   |
| <span data-ttu-id="2e9ad-158">classificationResults</span><span class="sxs-lookup"><span data-stu-id="2e9ad-158">classificationResults</span></span> | <span data-ttu-id="2e9ad-159">coleção [classificationResult](../resources/classificationresult.md)</span><span class="sxs-lookup"><span data-stu-id="2e9ad-159">[classificationResult](../resources/classificationresult.md) collection</span></span> | <span data-ttu-id="2e9ad-160">Contém o conjunto de resultados de classificação retornado pelo ponto de extremidade de classificação de dados.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-160">Contains the set of classification results returned by the data classification endpoint.</span></span> <span data-ttu-id="2e9ad-161">As informações de classificação são usadas para determinar o rótulo apropriado com base na configuração de rótulo de política de proteção de informações da Microsoft no centro de segurança e conformidade do Office 365.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-161">Classification information is used to determine the appropriate label based on the Microsoft Information Protection policy label configuration in Office 365 Security and Compliance Center.</span></span> |

## <a name="response"></a><span data-ttu-id="2e9ad-162">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e9ad-162">Response</span></span>

<span data-ttu-id="2e9ad-163">Se tiver êxito, este método retornará um `200 OK` código de resposta e um novo objeto da coleção [informationProtectionAction](../resources/informationprotectionaction.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-163">If successful, this method returns a `200 OK` response code and a new [informationProtectionAction](../resources/informationprotectionaction.md) collection object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2e9ad-164">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2e9ad-164">Examples</span></span>

<span data-ttu-id="2e9ad-165">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-165">The following example shows how to call this API.</span></span>

### <a name="request"></a><span data-ttu-id="2e9ad-166">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2e9ad-166">Request</span></span>

<span data-ttu-id="2e9ad-167">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-167">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2e9ad-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="2e9ad-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "informationprotectionlabel_evaluateclassificationresults"
}-->

```http
POST https://graph.microsoft.com/beta/informationprotection/policy/labels/evaluateClassificationResults
Content-type: application/json
User-agent: ContosoLOBApp/1.0

{
  "contentInfo": {
    "@odata.type": "#microsoft.graph.contentInfo",
    "format@odata.type": "#microsoft.graph.contentFormat",
    "format": "default",
    "identifier": null,
    "state@odata.type": "#microsoft.graph.contentState",
    "state": "rest"
  },
  "classificationResults": [
    {
      "sensitiveTypeId": "cb353f78-2b72-4c3c-8827-92ebe4f69fdf",
      "count": 4,
      "confidenceLevel": 75
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="2e9ad-169">C#</span><span class="sxs-lookup"><span data-stu-id="2e9ad-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/informationprotectionlabel-evaluateclassificationresults-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2e9ad-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2e9ad-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/informationprotectionlabel-evaluateclassificationresults-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2e9ad-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2e9ad-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/informationprotectionlabel-evaluateclassificationresults-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2e9ad-172">Resposta</span><span class="sxs-lookup"><span data-stu-id="2e9ad-172">Response</span></span>

<span data-ttu-id="2e9ad-173">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-173">The following is an example of the response.</span></span>

> <span data-ttu-id="2e9ad-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2e9ad-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "@odata.type": "#microsoft.graph.applyLabelAction",
      "responsibleSensitiveTypeIds": [
        "cb353f78-2b72-4c3c-8827-92ebe4f69fdf"
      ],
      "actionSource": "automatic",
      "label": {
        "id": "722a5300-ac39-4c9a-88e3-f54c46676417",
        "name": "Top Secret",
        "description": "",
        "color": "#000000",
        "sensitivity": 13,
        "tooltip": "This information is Top Secret.",
        "isActive": true
      },
      "actions": [
        {
          "@odata.type": "#microsoft.graph.protectByTemplateAction",
          "templateId": "0e7fea72-7bba-4438-a070-95c292cd6f8c"
        },
        {
          "@odata.type": "#microsoft.graph.metadataAction",
          "metadataToRemove": [],
          "metadataToAdd": [
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Enabled",
              "value": "true"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SetDate",
              "value": "2019-10-03T21:50:20Z"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Method",
              "value": "Standard"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_Name",
              "value": "Top Secret"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_SiteId",
              "value": "cb46c030-1825-4e81-a295-151c039dbf02"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ActionId",
              "value": "76dc494e-6c59-43e6-88a1-0000edd58fca"
            },
            {
              "name": "MSIP_Label_722a5300-ac39-4c9a-88e3-f54c46676417_ContentBits",
              "value": "8"
            }
          ]
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "informationProtectionLabel: evaluateClassificationResults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


